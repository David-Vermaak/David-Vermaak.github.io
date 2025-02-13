---
layout: post
  title: Python Desktop App
  description:  I created this app to streamline my own workflow. Over the course of the next 2 years it grew into a multifunctional productivity app.
  skills: 
    - Python
    - Desktop App
    - Compilation
    - Automation
  main-image: /eft_emails_dark.jpg
---
## EFT Emails

### Program Information

Welcome to the EFT Email Template Generator
How to Use:

1.) Select a Template: Choose a template from the dropdown

2.) Enter the client information

3.) Press submit

For the Recurring Emails and the Email Notices there will be a next tab that will take you to the next email template.

If you have a preformatted email from the client as a document you can use the "Convert Word File" or "Sanitize Text" option

How to Use **Convert Word File**:

1. ) Open the Word Document by clicking the button
2. ) Follow the prompts to add in any image URLs
3. ) Make sure to check the format of the result as formatting can be broken.

How to Use **Sanitize Text:**

1. ) Copy and paste the text from the document
2. ) Press submit
3. ) Make sure to check the format of the result as characters might be missing and formatting is often broken.

The HTML output converts the plaintext into:

paragraph tags: `<p></p>`

linebreak tags: `<br/>`

numbered lists:

1. bannana
2. potatoes

(from 1. bannana 2. potatoes)

lists:

* bannana
* potatoes

(from \* bannana \* potatoes)

website links: [https://1sourceonline.com/](https://1sourceonline.com/)

image links: {% include image-gallery.html images="EFT_logo.png" %}

If you have questions or concerns please contact me at [vermaak_d@icloud.com](mailto:vermaak_d@icloud.com)

## Compiling the .exe

make sure that nuitka is installed:

```bash
pip install nuitka
```

Then run this command in the termainal (within the project folder)

```bash
python -m nuitka main.py  
```

All the Command flags are at the top of the file and will be parsed automatically

```python
# nuitka-project: --onefile
# nuitka-project: --enable-plugin=tk-inter
# nuitka-project: --include-data-files={MAIN_DIRECTORY}/email.ico=email.ico
# nuitka-project: --windows-console-mode=disable
```

## Walk-through of Application:

### Menu in dark mode

{% include image-gallery.html images="eft_emails_dark.jpg" %}

### Menu in light mode

{% include image-gallery.html images="eft_emails_light.jpg" %}

### Email Selection

{% include image-gallery.html images="VTE_dark.jpg" %}

### Example Data

{% include image-gallery.html images="VTE_dark_example.jpg" %}

### Information Example

{% include image-gallery.html images="VTE_dark_example2.jpg" %}

### Text Email

{% include image-gallery.html images="VTE_dark_example3.jpg" %}

### HTML Email

{% include image-gallery.html images="VTE_dark_example4.jpg" %}

### Convert Word Doc

{% include image-gallery.html images="WordDocConverter.png" %}

### Sanitize Text

{% include image-gallery.html images="SanitizeText.png" %}
