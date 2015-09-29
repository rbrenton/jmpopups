# API

## $.setupJMPopups(`options`)

### Description

This method sets up the Plugin.

### Options

* **screenLockerBackground**: (String)<br/>
This property sets the color of the screenlocker.<br />
*Default value*: `"#000000"`

* **screenLockerOpacity**: (String)<br/>
This property sets the opacity of the screenlocker<br />
*Default value*: `"0.5"`

<br />
<br />
<br />



## $.openPopupLayer(`options`)

### Description

This method opens a Popup.

### Options

* **name**: (String)<br/>
This property sets the name of the popup. It's a mandatory property and should be unique.<br />
*Example*: `"contactForm"`
   
* **width**: (int)<br/>
This property sets the width of the popup.<br />
*Default value*: `"auto"`<br />
*Example*: `300`

* **height**: (int)<br/>
This property sets the width of the popup.<br />
_Default value_: `"auto"`<br />
*Example*: `200`

* **target**: (String)<br/>
This property sets the id of the html element that contains the content to be used.<br />
If you set this property, the popup will COPY the content of the element and it will ignore the url and parameters properties.<br />
*Example*: `"myDiv"`

* **url**: (String)<br/>
This property sets the url to be used in the ajax request.<br />
*Example*: `"contact_popup.html"`

* **parameters**: (Object - Map)<br/>
This property sets the parameters to be used in the ajax request (get),<br />
*Default value*: `{}`<br />
*Example*: `{id:123, user:"guest"}`

* **cache**: (Boolean)<br/>
If false it will force the page that you requested not to be cached by the browser.<br />
*Default value*: `false`

* **success**: (Function)<br/>
This function will be called when the popup loads.<br />
*Default value*: `function() {}`

* **error**: (Function)<br/>
This function will be called if an ajax error happens.<br />
*Default value*: `function() {}`

* **beforeClose**: (Function)<br/>
This function will be called before the popup closes.<br />
*Default value*: `function() {}`

* **afterClose**: (Function)<br/>
This function will be called after the popup closes.<br />
*Default value*: `function() {}`

<br />
<br />
<br />

## $.closePopupLayer(`[name]`)

### Description

This method closes a Popup.

### Arguments

* **name**: (String)<br/>
The Popup name to be closed.<br />
If not set, it will close the last Popup opened.

<br />
<br />
<br />

## $.reloadPopupLayer(`[name[, callback]]`)

### Description

This method reloads a Popup.

### Arguments

* **name**: (String)<br/>
The Popup name to be reloaded.<br />
If not setted, it will reload the last Popup opened.

* **callback**: (Function)<br/>
This function will be called after the popups reloads.
It will be executed after the success() method.
