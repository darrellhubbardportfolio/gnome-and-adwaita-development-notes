is the interactive part of the gnome application.

## Creating an ApplicationWindow
to create a new window, we have two meethod:
## new()
let's us build the item right out of the box, without defining the properties. later on we can add the properties. below is how to configure the properties with this **constructor** method first.
### properties
these are considered 
#### instance methods
- window_get_id()
- window_get_show_menubar()
- window_set_show_menubar()
#### instance methods from gtk window
- window_close()
- window_destroy()
- window_fullscreen()
- window_get_application()
- window_get_focus()
- window_get_focus_visible()
- window_get_resizable()
- window_get_title()
- window_get_titlebar()
- window_maximize()
- window_minimize()
- window_set_default_size()
- window_set_hide_on_close()
- window_set_title()
- window_set_titlebar()
- 

## builder()
acts like a form that contains a list of properties that we want to add to our component before actually building it.
### properties
