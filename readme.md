Material Design skin for Webix UI
=================================

[![Join the chat at https://gitter.im/webix-hub/webix](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/webix-hub/webix) 


Live demo - http://webix.com/demos/material/admin-app/index.html#!/app/forms

Skin will work with Webix 2.3+

How to use
-----------

- copy files into `codebase` folder of Webix UI package
- use skin file on page as any other skin

```html
<html>
<head>
	<script type="codebase/webix.js"></script>
	<link rel="stylesheet" type="text/css" href="codebase/skins/material.css">
</head>
<body>
webix.ready(function(){
	//some webix related UI here
});
</body>
</html>
```

Shared CSS classes
------------------

Example - http://webix.com/demos/material/admin-app/index.html#!/app/typography

### Text and Background

- text_primary
- text_info
- text_success
- text_warning
- text_danger
- text_muted

```js
webix.ui({
	rows:[{
		template:"Some text",
		css:"text_info"
	},{
		template:"Some background",
		css:"bg_danger"
	})
```

### Buttons

- button_primary
- button_info
- button_success
- button_warning
- button_danger
- button_transparent
- button_raised

```js
webix.ui({
	view:"button",
	css:"button_success button_raised"
})
```


### Icons

- solid_icon
- action_icon
- danger_icon

```js
webix.ui({
	view:"icon",
	icon:"users",
	css:"solid_icon"
});
```


### Panels

- bg_clean
- bg_panel
- bg_panel_raised

```js
webix.ui({
	rows:[
		{ template:"A" },
		{ template:"B", css:"bg_panel"},
		{ template:"C" }
	]
})
```

Material layout
------------------

Skin adds one more type of layout.

```js
webix.ui({
	type:"material",
	rows:[
		{ template:"A" },
		{ template:"B" },
		{ template:"C" }
	]
})
```

This type of layout shows all content elements as material panels. 


License
---------

Code is released under the MIT License:

Copyright (c) 2015

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
