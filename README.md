Bootstrap Shortcodes for WordPress
===

This is a plugin for WordPress that adds shortcodes for easier use of the Bootstrap elements in your content.

## Requirements
This plugin won't do anything if you don't have website built with the [Twitter Bootstrap framework](http://getbootstrap.com/). **The plugin does not include the Bootstrap framework**.

The plugin is tested to work with ```Bootstrap version 3.0.0``` and ```WordPress 3.6```.

## Installation
To install this plugin, just download it, and drop the folder in the ```wp-content/plugins/```. Then login to WordPress and activate the plugin.

## Supported shortcodes
The plugin doesn't support all Bootstrap elements yet, but most of them.

* [Grid](#grid)
* [Buttons](#buttons)
* [Button Groups](#button-groups)
* [Alerts](#alerts)
* [Code](#code)
* [Labels](#labels)
* [Badges](#badges)
* [Icons](#icons)
* [Tables](#tables)
* [Accordion](#accordion)
* [List Groups](#list-groups)
* [Tabs](#tabs)
* [Wells](#wells)
* [Panels](#panels)


## Usage

### Buttons
	[button type="success" size="lg" link="#"] … [/button]

Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
type | The type of the button | optional | default, primary, success, info, warning, danger, link | default
size | The size of the button | optional | xs, sm, lg | none
xclass | Any extra classes you want to add | optional | Any text | none
link | The url you want the button to link to | optional | any valid link | none

[Bootstrap button documentation](http://getbootstrap.com/css/#buttons)

### Button Groups
	[button-group]
        [button link="#"] … [/button]
        [button link="#"] … [/button]
        [button link="#"] … [/button]
	[/button-group]

[Bootstrap button groups documentation](http://getbootstrap.com/css/#btn-groups)

### Alerts
	[alert type="success"] … [/alert]

Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
type | The type of the alert | required | success, info, warning, danger | success
dismissable | If the alert should be dismissable | optional | true, false | false
strong | Text to display in bold at the beginning | optional | Any text | false

[Bootstrap alert documentation](http://getbootstrap.com/components/#alerts)

### Code
	[code] … [/code]

Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
inline | display inline code | optional | true, false | false
scrollable | set a max height of 350px and provide a scroll bar. Not usable with inline="true".  | optional | true, false | false

[Bootstrap code documentation](http://getbootstrap.com/css/#code)

### Labels
	[label type="success"] … [/label]

Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
type | the type of label to display | optional | default, primary, success, info, warning, danger | default

[Bootstrap label documentation](http://getbootstrap.com/components/#labels)

### Badges
	[badge right="true"] … [/badge]

Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
right | Whether the badge should align to the right of its container | optional | true, false | false

[Bootstrap badges documentation](http://getbootstrap.com/components/#badges)

### Wells
	[well size="small"] … [/well]

Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
size | Modifies the amount of padding inside the well | optional | sm, lg | normal

[Bootstrap wells documentation](http://getbootstrap.com/components/#wells)

### Panels
	[panel type="info" title="Panel Title" footer="Footer text"] … [/panel]

Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
type | The type of the panel | optional | default, primary, success, info, warning, danger, link | default
title | The panel title | required | Any text | none
footer | The panel footer text if desired | optional | Any text | none

[Bootstrap panels documentation](http://getbootstrap.com/components/#panels)

### Icons
	[icon type="arrow"]

Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
type | The type of icon you want to display | required | See Bootstrap docs | none

[Bootstrap Glyphicons documentation](http://getbootstrap.com/components/#glyphicons)

### Grid
	[row]
	  [column medium="6"]
	    …
	  [/column]
	  [column medium="6"]
	    …
	  [/column]
	[/row]

Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
xs | size of column on extra small screens (<768px) | optional | 1-12 | false
sm | size of column on small screens (≥768px) | optional | 1-12 | false
md | size of column on medium screens (≥992px) | optional | 1-12 | false
lg | size of column on large screens (≥1200px) | optional | 1-12 | false

[Bootstrap grid documentation](http://getbootstrap.com/css/#grid).

### Tables
	[table type="striped" cols="#,First Name, Last Name, Username" data="1, Filip, Stefansson, filipstefansson, 2, Victor, Meyer, Pudge, 3, Måns, Ketola-Backe, mossboll"]

### Accordion
	[collapsibles]
	  [collapse title="Collapse 1" state="active"]
	    …
	  [/collapse]
	  [collapse title="Copllapse 2"]
	    …
	  [/collapse]
	  [collapse title="Copllapse 3"]
	    …
	  [/collapse]
	[/collapsibles]
    
### List Groups
	[list-group]
	  [list-group-item]
	    …
	  [/list-group-item]
	  [list-group-item]
	    …
	  [/list-group-item]
	  [list-group-item]
	    …
	  [/list-group-item]
	[/list-group]

[Bootstrap list groups documentation](http://getbootstrap.com/components/#list-group)

### Tabs
	[tabs]
	  [tab title="Home"]
	    …
	  [/tab]
	  [tab title="Profile"]
	    …
	  [/tab]
	  [tab title="Messages"]
	    …
	  [/tab]
	[/tabs]