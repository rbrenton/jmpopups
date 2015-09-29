==$.setupJMPopups(`options`)==

===Description:===
    This method sets up the Plugin.

===Options:===
    * *screenLockerBackground*: (String)
        This property sets the color of the screenlocker.<br />
        _Default value_: "#000000"

    * *screenLockerOpacity*: (String)
        This property sets the opacity of the screenlocker<br />
        _Default value_:"0.5"

<br /><br /><br />




==$.openPopupLayer(`options`)==

===Description:===
    This method opens a Popup.

===Options:===
    * *name*: (String)
        This property sets the name of the popup. It's a mandatory property and should be unique.<br />
        _Example_: "contactForm"
   
    * *width*: (int)
        This property sets the width of the popup.<br />
        _Default value_: "auto"<br />
        _Example_: 300

    * *height*: (int)
        This property sets the width of the popup.<br />
        _Default value_: "auto"<br />
        _Example_: 200

    * *target*: (String)
        This property sets the id of the html element that contains the content to be used.<br />
        If you set this property, the popup will COPY the content of the element and it will ignore the url and parameters properties.<br />
        _Example_: "myDiv"

    * *url*: (String)
        This property sets the url to be used in the ajax request.<br />
        _Example_: "contact_popup.html"

    * *parameters*: (Object - Map)
        This property sets the parameters to be used in the ajax request (get),<br />
        _Default value_: {}<br />
        _Example_: {id:123, user:"guest"}

    * *cache*: (Boolean)
        If false it will force the page that you requested not to be cached by the browser.<br />
        _Default value_: false

    * *success*: (Function)
        This function will be called when the popup loads.<br />
        _Default value_: function() {}

    * *error*: (Function)
        This function will be called if an ajax error happens.<br />
        _Default value_: function() {}

    * *beforeClose*: (Function)
        This function will be called before the popup closes.<br />
        _Default value_: function() {}

    * *afterClose*: (Function)
        This function will be called after the popup closes.<br />
        _Default value_: function() {}

<br /><br /><br />



==$.closePopupLayer(`[name]`)==

===Description:===
    This method closes a Popup.

===Arguments:===
    * *name*: (String)
        The Popup name to be closed.<br />
        If not set, it will close the last Popup opened.

<br /><br /><br />



==$.reloadPopupLayer(`[name[, callback]]`)==

===Description:===
    This method reloads a Popup.

===Arguments:===
    * *name*: (String)
        The Popup name to be reloaded.<br />
        If not setted, it will reload the last Popup opened.

    * *callback*: (Function)
        This function will be called after the popups reloads.
        It will be executed after the success() method.