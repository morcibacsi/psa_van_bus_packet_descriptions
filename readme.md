# PSA VAN Bus packet descriptions

This repository contains the descriptions of the VAN bus packets.

It is based on Graham Auld's findings and the VAN_Frames.txt which was originated from the rt3wiki page which ceased to exists. Most of the packets were verified and reviewed and additional findings have been added.

## Project structure

The project is basically a web page and the **packet descriptions are inside files with .json extension**. Every iden has its own file inside the data folder. Some packets can have different lengths based on some conditions (year of manufacture, meaning of the packet). In these cases I separated the descriptors into different files.

The **html file** contains **only the design** of the page. When opened it loads the json files with an ajax request and displays their contents. It uses bootstrap, jquery, and the [mustache.js][mustache_js] library to parse the json files.

A live version can be found on my page [on this link][live_version].

[![Click to open the live version](http://pinterpeti.hu/psavanbus/preview.png)](http://pinterpeti.hu/psavanbus/PSA-VAN.html "Click to open the live version")

## Thanks

I would like to thank Graham Auld. Without [his page][graham_auld] this project would never exists.

[live_version]: http://pinterpeti.hu/psavanbus/PSA-VAN.html
[graham_auld]: http://graham.auld.me.uk/projects/vanbus/packets.html
[mustache_js]: https://github.com/janl/mustache.js

