designing modern-day applications with gtk4 and adwaita. think of adwaita as the css version of gtk4. you may not find all components in the adwaita docs, but you will find some components in the gtk4 documentaion.
because i love rust and it's intelligence when coming to auto handling memory management, i will use it to code in. but i also will create content for python developers aswell too; i mean python is almost a universal coding langauage that most of us probably have picked up.

anyway, if we visit crates.io, we can add the the following packages to our application:
gtk4-rs
libadwaita

in all applications that we build, its probably best if we think about approaching the layout of our application before adding components. So a simple design would be nice before actually implementing our application. while doeing this i will only regard layout components in the other files.

every component has two wasy that it can build, you can use the **::builder()** method or you can just use a constructor to create it such like **::new()** for must components because they can vary.

```
use gtk4 as gtk;
use gtk4::prelude::*;
use gtk4::{Application, ApplicationWindow};

fn main()-> ApplicationWindow {

	// create the application
	let app = Application::builder()
		.application_id("hello-world")
		.build();
		
	// this window belongs to the application above
	let window = ApplicationWindow::builder()
		.application(app)
		.application_title("hello world!")
		.build();
		
	// return the application and run it
	window
}
```
above is just an example of using the builder method. the constructor method, just requires a constructor. then later on in the application, we call the reference of the variable for that component and then append the function to it. that's all. i prefer the builder method, to do everything at once.
