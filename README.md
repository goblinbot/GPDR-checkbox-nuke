# GPDR-checkbox-nuke
Uncheck all checkboxes. No exceptions.

Is this petty? Yes. But websites like Tumblr have decided that a button to "uncheck all checkboxes" is not needed, and they'd rather have you manually unselect 99999 advertisers. 

So, here is a simple javascript bit you can copypaste into your console to unselect EVERY checkbox on the website.

_______________

var checkboxes = new Array(); 
  checkboxes = document.getElementsByTagName('input');
 
  for (var i=0; i<checkboxes.length; i++)  {
    if (checkboxes[i].type == 'checkbox')   {
      checkboxes[i].checked = false;
    }
  }
