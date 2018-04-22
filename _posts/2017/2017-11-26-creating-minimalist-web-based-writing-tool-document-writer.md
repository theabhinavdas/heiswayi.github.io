---
layout: post
title: Creating a minimalist web-based writing tool
description: Document Writer is a minimalist web-based writing tool to easily write document using web browser and save it as a plain text, HTML or markdown format file.
keywords: minimalist, web-based app, writing tool, document writer
tags: [PHP, JavaScript, AJAX, jQuery, Project]
comments: true
---

This weekend, I have been spending some of my times creating a minimalist web-based tool called [**Document Writer**](https://nrird.xyz/document-writer). Document Writer is very simple web-based writing tool to easily write document by using a web browser and save the written document into a plain text, HTML or markdown format file.

The **reason** behind this web tool is because I need to write document easier and faster with the help of [TinyMCE editor plugin](https://www.tinymce.com/), then I can save it into the format I needed (HTML or markdown, mostly), without the need for me to manually write the HTML code.

### Screenshot

![Screenshot](https://i.imgur.com/3FRdl5R.png)

**Web Address:** [https://nrird.xyz/document-writer](https://nrird.xyz/document-writer)

### What you can do with this web tool?

Just by using your web browser, you can simply write something in the editor, craft your document, upload your image files and save it as a plain text, HTML or markdown format file into your local computer.

### How this web tool is created, technically?

Document Writer is created using [Bootstrap v4.0.0](https://getbootstrap.com/) for the tool interface layout, [TinyMCE's JS editor plugin](https://www.tinymce.com/) to provide a nice editor interface and toolbars for writing, [FileSaver.js](https://github.com/eligrey/FileSaver.js/) to save the written document into a local file, [moment.js](http://momentjs.com/) for auto-define filename if left blank, [to-markdown.js](https://github.com/domchristie/to-markdown) for converting HTML code into a markdown format, [htmLawed](http://www.bioinformatics.org/phplabware/internal_utilities/htmLawed/) to tidy/auto-indent the HTML code that generated by TinyMCE plugin before saving into a HTML file and some custom scripts (jQuery & PHP) to handle AJAX or manage image upload service at server-side. Other that these, Document Writer also uses the [Web Storage API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API/Using_the_Web_Storage_API) for auto-save feature and recording of a list of uploaded image filenames into the server by the user.

User can download all uploaded images as an archive (.zip) or delete all the image files immediately from the server. However, each files stored on the server will be automatically deleted after 24 hours of creation time.

_If you have any inquiry such as a question to ask, problem/bug to report, idea or suggestion related to this web tool, feel free to send me an email at [hnrird@gmail.com](mailto:hnrird@gmail.com)._