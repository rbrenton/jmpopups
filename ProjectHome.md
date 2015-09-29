# Description #
A JQuery Plugin for popups layers.

<br />
# Advantages #
  * You can open more than one popup the same time;
  * There is no pre-defined layout, so you are able to create your own layout;
  * You can call the popups using ajax or using the content of a hidden html element;
  * The **jmpopups** is concerned about acessibility. When a popup is opened, the focus will be kept only inside that popup. It will directly focus the first focusable element. The idea is to help users who use the keyboard for browsing (f.e. disabled people).
  * It works for IE 6+, FF 1.5+, Opera 9.`*`, Chrome 2.`*`, Safari 4.`*`.
  * Compatible with JQuery 1.3.`*`

<br />
# Download #
http://jmpopups.googlecode.com/files/jquery.jmpopups-0.5.1.zip

<br />
# Demo #
http://otavioavila.com/jmpopups-example/

<br />
# API #
http://code.google.com/p/jmpopups/wiki/API

<br />
# Usage Example #
```
$.openPopupLayer({
	name: "contactForm",
	width: 300,
	url: "contact_form.html",
	success: function() {
		alert("It is loaded");
	}
});
```

<br />
# Questions or bugs? #
http://otavioavila.com