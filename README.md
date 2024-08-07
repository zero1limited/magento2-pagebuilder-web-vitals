# Magento 2 - PageBuilder Web Vitals (With Lazyload Tags)

For Magento 2.4.3

## Description

Magento's Page Builder is a great core module (as of 2.4.3), which makes it easy to create content-rich pages, but there are a couple of elements that are missing:

- Image dimensions
- Link labels
- loading="lazy" tags

Why are these important?...

Google's Web Vitals audits contain improvement suggestions that help increase both the Performance and Accessibility metrics. The 2 relating to Magento's Page Builder are:

- Image elements do not have explicit width and height
- Links do not have a discernible name

**Image elements do not have explicit width and height**

Once this module is installed, you will have 2 new fields allowing you to add a width and height to each image you upload via Page Builder. Adding these dimensions will ensure that the image you have uploaded will pass the Google Web Vital audit

**Links do not have a discernible name**

This is recommended by Google when a tags don't contain text. When adding an image with a link, the a tag only contains an image, but one way to ensure this a tag passes the Web Vitals audit is to add an aria-label tag to the link itself.
Once this module is installed, you will have a new field allowing you to add a label to the link tag which will ensure the link passes the audit.

Adding image dimensions and link labels will ensure those elements pass the audit, but it can also have a knock on effect that also helps improve your CLS score (Content Layout Shift)

## Installation...

```
composer require zero1/module-pagebuilder-web-vitals
```

© Zero-1 Ltd | [www.zero1.co.uk](https://www.zero1.co.uk/)
