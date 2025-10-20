[![License: CC0-1.0](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)

# Verona Interfaces: Specification for Widget

In order to understand Verona Interfaces, please go
to [Verona Interfaces Introduction](https://verona-interfaces.github.io)!

A Verona Widget is a Html-file to be loaded into an iframe element of a web application. We call the web application "host". This specification describes the asynchronous communication between a host and the widget.

Read the spec here:
* [Html-Document](https://verona-interfaces.github.io/widget)
* [AsyncApi source yaml](widgetapi.yaml)

The widget file must contain of one script tag for metadata as json-ld. The syntax and elements are described [here](https://verona-interfaces.github.io/intro/metadata).

## release notes

Please see the [release section](https://github.com/verona-interfaces/widget/releases) of this repository to learn about changes.

## For Contributors

This api is written as [async api](https://www.asyncapi.com/de) yaml file. After committing to main branch, a GitHub action is triggered to build the html page. Don't forget to update the version. Then, create an release that matches the version of the yaml file.

If you like to check the yaml file or the html page before committing to main branch, 

* have an npm/node.js-environment installed
* check out the repo
* run `npm install`
* run the `generate` script in package.json.

After that, you can check `public/index.html` in a browser. This file will be ignored by git.