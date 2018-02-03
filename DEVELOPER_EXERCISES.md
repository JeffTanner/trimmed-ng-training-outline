[Full Training Outline](./README.md)


### LEGEND
__M__ Developer

__PREP__: Each person should have an Angular/Typscript BP created from the generator with all dependencies installed and ready to go. 

Modules to cover from Fundamentals on Angular.io:
## Architecture
* __EXERCISE__: No exercies. This section should be purely an overview/introduction to topics that will be covered in more detail throughout the course

## Template & Data Binding
* Displaying Data
	* __M__ Showing component properties with interpolation
	* __M__ Template inline or template file
	* __M__ Constructor or variable initialization
	* __M__ Showing an array property with *ngFor
	* __M__ Creating a class for the data
	* __M__ Conditional display with *ngIf
	* Summary
* Template Syntax
	* __M__ Template Expressions
		* __M__ Expression context
		* __M__ Expression guidelines
	* __M__ Template Statements
		* __M__ Statement context
		* __M__ Statement guidelines
	* __M__ Binding syntex: An overview
		* __M__ A new mental model
		* __M__ HTML attribute vs. DOM property
		* __M__ Binding targets
	* __M__  Property binding ( [property] )
		* __M__ One-way in 
		* __M__ binding target
		* __M__ Avoid side effects
		* __M__ Return the proper type
		* __M__ Remember the brackets
		* __M__ One-time string initialization
		* __M__ Property binding or interpolation?
	* __M__ Attribute, class, and style bindings
		* __M__ Attribute binding
		* __M__ Class binding
		* __M__ Style binding
	* __M__ Event binding ( (event) )
		* __M__ Target event
		* __M__ $event and event handling statements
		* __M__ Custom events with EventEmitter
		* __M__ Template statements have side effects
	* __M__ Two-way binding ( [(…))] )
	* Built-in directives
	* __M__ Built-in attribute directives
		* __M__  ngClass
		* __M__  ngStyle
		* __M__  ngModel - two-way binding to form elements with [(ngModel)]
	* __M__ Built-in structural directives
		* __M__ ngIf
		* __M__ ngForOf
		* __M__ Template input variables
		* __M__ The ngSwitch directive
	* __M__  Template reference variables (#var)
	* __M__ Input and output properties
		* __M__ Binding to a different component
		* __M__ Declaring Input and Output properties
		* __M__ Input or output?
		* __M__ Aliasing input/output properties
	* __M__ Template expression operators
		* __M__ The pipe operator ( | )
		* __M__ The safe navigation (?.) and null property paths
		* __M__ The non-null assertion operator ( ! )
* Lifecycle Hooks
	* __M__ Component lifecycle hooks overview
	* __M__ Lifecycle sequence
	* __M__ Interfaces are optional (technically)
		* __M__ OnInit()
		* __M__ OnDestroy()
	* __M__ OnChanges()
	* __M__ DoCheck()
	* __M__ AfterView
		* __M__ Abide by the unidirectional data flow rule
	* __M__ AfterContent
		* __M__ Content projection
		* __M__ AfterContent hooks
		* __M__ No unidirectional flow worries with AfterContent
* Component Interaction
	* __M__ Intercept input property changes with a setter
		* _Previous section on OnChanges covers what  needs* to be covered, this just gives a little more detail_
	* Parent listeners for child event
		* _Previous section on Input and Output properties* covers enough of this, this just gives more detail_
	* __M__ Parent interacts with child via local variable
	* __M__ Parent calls an @ViewChild()
	* __M__ Parent and children communicate via a service
* __M__   Component Styles
	* __M__  Using component styles
	* __M__  Style scope
	* __M__  Special selectors
		* __M__  :host
		* __M__  :host-context
	* __M__  Loading component styles
		* __M__  Styles in component metadata
		* __M__  Style files in component metadata
		* __M__  Template inline styles
		* __M__  Template link tags
		* __M__  CSS @imports
		* __M__  External and global style files
		* __M__  Non-CSS style files
	* __M__  View encapsulation
	* __M__  Inspecting generated CSS
* __M__ Attribute Directives
	* __M__ Directives overview
	* __M__ Build a simple attribute directive
		* __M__ Write the directive code
	* __M__ Apply the attribute directive
	* __M__ Respond to user-initiated events
	* __M__ Pass values into the directive with an @Input data* binding
		* __M__ Binding to an @Input property
		* __M__ Bind to an @Input alias
	* __M__ Write a harness to try it
	* __M__ Bind to a second property
	* Summary
		* Appendix: Why Add @Input?
* __M__ Pipes
	* __M__ Using pipes
	* __M__ Built-in pipes
	* __M__ Parameterizing a pipe
	* __M__ Chaining pipes
	* __M__ Custom pipes
	* __M__ The PipeTransform interface
	* Next steps
	* __M__ Appendix: No FilterPipe or OrderByPipe
## Forms
* __M__ User Input
	* Binding to user input events
	* __M__ Get user input from the $event object
		* __M__ Type the $event
		* __M__ Passing $event is a dubious practice
	* __M__ Key event filtering (with key.enter)
	* On blur
	* Source code
	* Summary
## Bootstrapping
* __M__ The declarations array
	* __M__ Using directives with @NgModule
* __M__ The imports array
* __M__ The providers array
* __M__ The bootstrap array
* __M__ More about Angular modules
## NgModules
* __M__ JS Modules vs NgModules
	* __M__ JavaScript modules
	* __M__ NgModules
	* __M__ More on NgModules
* __M__ Frequently Used NgModules
	* __M__ Importing modules
	* __M__ BrowserModule and CommonModule
	* __M__ More on NgModules
* __M__ Entry Components
	* __M__ A bootstrapped entry component
	* __M__ A routed entry component
	* __M__ The entryComponents array
		* __M__ entryComponents and the compiler
	* __M__ More on Angular modules
* __M__ Feature Modules
	* __M__ Feature modules vs root modules
	* __M__ How to make a feature module
	* __M__ Importing a feature module
	* __M__ Rendering a feature module's component template
	* __M__ More on NgModules
* Providers
	* __M__ Create a service
	* __M__ Provider scope
* __M__ Sharing NgModules
	* __M__ Using components vs services from other modules
	* __M__ More on NgModules
## Dependency Injection
	* _This topic seems to already be covered quite a bit in the other material, so this section is optional_
* DI in Action
	* __M__ Application-wide dependencies
	* __M__ External module configuration
	* __M__ @Injectable() and nested service dependencies
		* __M__ @Injectable()
	* __M__ Limit service scope to a component subtree
		* __M__ Take a break!
## HttpClient
* __M__ Setup: installing the module
* __M__ Making a request for JSON data
	* __M__ Typechecking the response
	* __M__ Reading the full response
	* __M__ Error Handling
	* __M__ Requesting non-JSON data
## Routing & Navigation
* __M__ Overview
* __M__ The basics
	* __M__ <base href>
	* __M__ Router imports
	* __M__ Configuration
	* __M__ Router outlet
	* __M__ Router links
	* __M__ Router state
	* __M__ Activated route
	* __M__ Router events
	* __M__ Summary
	* __M__ Redirecting routes
	* __M__ Module import order matters
	* __M__ Route definition with a parameter
	* __M__ Setting the route parameters in the list view
	* __M__ Child route configuration
	* __M__ Relative navigation
* __M__ Migrating URLs with Redirects
	* __M__ Changing /heroes to /superheroes
* Inspect the router's configuration
* Wrap up and final app 
