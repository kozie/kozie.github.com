---
layout: post
title: "Quickly generate transparent png as data URI"
description: ""
category: HTML5/JS
tags: []
---
{% include JB/setup %}

For quick image placeholders or IE background fixes i usually generate a Data URI image through Chrome's console like so.

	// Create temp canvas
	var c = document.createElement('canvas');

	// Set a width and height
	c.width = 75;
	c.height = 75;

	// Now generate the Data URI
	c.toDataURL();

The above code will eventually return the Data URI of a 75 by 75 transparent PNG in your console.
Click the link to open it in a new tab and copy the URL from your address bar or simply right-click the link and copy it from there.

You can (for example) the URI like so

	<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEsAAABLCAYAAAA4TnrqAAAA7klEQVR4Xu3SsQ0AAAjDMPj/aV4guztnsrpjb4F9l8KBFU4AC1YQCKlnwQoCIfUsWEEgpJ4FKwiE1LNgBYGQehasIBBSz4IVBELqWbCCQEg9C1YQCKlnwQoCIfUsWEEgpJ4FKwiE1LNgBYGQehasIBBSz4IVBELqWbCCQEg9C1YQCKlnwQoCIfUsWEEgpJ4FKwiE1LNgBYGQehasIBBSz4IVBELqWbCCQEg9C1YQCKlnwQoCIfUsWEEgpJ4FKwiE1LNgBYGQehasIBBSz4IVBELqWbCCQEg9C1YQCKlnwQoCIfUsWEEgpJ4FKwiE9ABv7ABMaoSFhQAAAABJRU5ErkJggg==" alt="75 by 75 transparent PNG" width="75" height="75" />