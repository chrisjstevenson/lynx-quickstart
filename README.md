# Lynx Quick Start

This goals for this project are
- Provide a working server and client to assist with learning the [lynx media type](#lynx-media-type)
- Provide [lynx-docs](https://www.npmjs.com/package/@lynx-json/lynx-docs) templates that illustrate concepts within the [lynx media type](#lynx-media-type)
- Provide examples of [lynx-docs](https://www.npmjs.com/package/@lynx-json/lynx-docs) authoring concepts
- Provide a customizable sample HTML/JavaScript client that displays lynx documents in a browser

You may use this project in a couple of ways
- As a starting point for a new project
- As a learning tool to understand the [lynx media type](#lynx-media-type), authoring documents using [lynx-docs](https://www.npmjs.com/package/@lynx-json/lynx-docs), and customizing the display of those documents in a browser.

## Set-up and start
```
git clone https://github.com/lynx-json/lynx-quickstart.git
npm install
npm start
```

Open browser to [http://localhost:8080/client/index.html](http://localhost:8080/client/index.html)

## Lynx media type
Lynx (application/lynx+json) is a hypertext media type that was created to fit a perceived space between data formats with no connections (.json, .xml, etc.) and display formats (HTML, iOS, Android, etc.). A primary goal of Lynx is to separate process (hypertext) and information (data, metadata) from display, thereby allowing different display contexts (web, mobile, desktop, other) to present the information in a way appropriate for that medium. The separation further allows for the process and information to change separately from the display.

The media type specification can be found at [http://lynx-json.org/specification/](http://lynx-json.org/specification/).

## Authoring documents with lynx-docs
[lynx-docs](https://www.npmjs.com/package/@lynx-json/lynx-docs) is a Node.js package that provides an working web server and a set of transformation functions to convert specially crafted YAML documents into [lynx](#lynx-media-type) documents. It further allows for the modeling of dynamic data using data files that are bound to templates.

Details about configuring the server and authoring documents can be found in the [lynx-docs wiki](https://github.com/lynx-json/lynx-docs/wiki)

## Displaying documents
In order to display [lynx](#lynx-media-type) documents a user agent must understand the media type and how to convert the values found in the document into visualizations. This process is identical to how a browser understand the HTML media type and can turn an HTML document returned from a server into something more visual. 

Included in this project is an HTML and JavaScipt user agent that understands [lynx](#lynx-media-type) documents and knows how to transform those into HTML elements with interactions for display in a browser. 