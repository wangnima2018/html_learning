1 https://stackoverflow.com/questions/26061651/what-is-the-purpose-of-the-html-name-attribute
In an input element, the name attribute defines the name of the control.
Only controls that have a name can be “successful”, i.e. may contribute to the form data set sent to a server.
Thus, it is indispensable in order to make the value of the control submitted to server-side processing. 
The id attribute has nothing to do with this; it has its own uses, such as helping to associate a label with the control, as in the example.

Consequently, the name attribute is not needed if you need not have the control value submitted. 
For example, if you have a single submit button like <input type=submit value=Send>, you don’t need it;
but if you have several submit buttons and you need to recognize, server-side, which one was used, you need it.
If the form data is not sent to server-side processing but handled only in client-side processing, the name attribute is not used, 
as you can access the values with other means.
