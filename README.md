[Exercises for Developers](./DEVELOPER_EXERCISES.md)

May need to add a short module on what decorators are and what they do

Anything declared in the AppModule is available app wide, submodule declarations are only available to the declarable items connected with that specific module


Maybe before starting any other training, we create an app with angular-cli and go through and point out with a brief explanation all the pieces (decorators, services, components, routers, modules), then we go into the formal Angular training

Boilerplate routing should be setup with '**' redirecting to whatever '' is pointing to

Should cover some basic Typescript things, like interfaces
	• When you make it private in the constructor declaration it adds it to 'this'
Topic of observables needs to be covered briefly, just enough so they know how to subscribe to one so they can do what they need to do


### LEGEND
__M__ Developer

__D__ Designer

__DO__ Designer - overview concepts, no need to get deep into the content

__A__ Advanced Topic

__W__  Web specific

__H__ Helpful, but not required

Modules to cover from Fundamentals on Angular.io:
## Architecture
* __M__ Modules
	* __M__ NgModules vs. JavaScript modules
	* __M__ Angular libraries
* __M__ Components
* __M__ Templates
* __M__ Metadata
* __M__ Data binding
* __M__ Directives
* __M__ Services
* __M__ Dependency Injection
* __M__ Wrap Up
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
	* HTML in templates
	* Interpolation ( {{…}} )
	* __M__ __DO__ Template Expressions
		* __M__ __DO__ Expression context
		* __M__ __DO__ Expression guidelines
	* __M__ __DO__ Template Statements
		* __M__ __DO__ Statement context
		* __M__ __DO__ Statement guidelines
	* __M__ __DO__ Binding syntex: An overview
		* __M__ __DO__ A new mental model
		* __M__ __DO__ HTML attribute vs. DOM property
		* __M__ __DO__ Binding targets
	* __M__ __D__ Property binding ( [property] )
		* __M__ __DO__ One-way in 
		* __M__ __DO__ binding target
		* __M__ __DO__ Avoid side effects
		* __M__ __DO__ Return the proper type
		* __M__ __DO__ Remember the brackets
		* __M__ __DO__ One-time string initialization
		* __M__ __DO__ Property binding or interpolation?
	* __M__ __DO__ Attribute, class, and style bindings
		* __M__ __DO__ Attribute binding
		* __M__ __DO__ Class binding
		* __M__ __DO__ Style binding
	* __M__ Event binding ( (event) )
		* __M__ Target event
		* __M__ $event and event handling statements
		* __M__ Custom events with EventEmitter
		* __M__ Template statements have side effects
	* __M__ Two-way binding ( [(…))] )
	* Built-in directives
	* __M__ __DO__ Built-in attribute directives
		* __M__ __D__ ngClass
		* __M__ __D__ ngStyle
		* __M__ __D__ ngModel - two-way binding to form elements with [(ngModel)]
	* __M__ Built-in structural directives
		* __M__ ngIf
		* __M__ ngForOf
		* __M__ Template input variables
		* __M__ The ngSwitch directive
	* __M__ __D__ Template reference variables (#var)
	* __M__ Input and output properties
		* __M__ Binding to a different component
		* __M__ Declaring Input and Output properties
		* __M__ Input or output?
		* __M__ Aliasing input/output properties
	* __M__ Template expression operators
		* __M__ The pipe operator ( | )
		* __M__ The safe navigation (?.) and null property paths
		* __M__ The non-null assertion operator ( ! )
	* __A__ The $any type cast function ($any(<expression>)
* Lifecycle Hooks
	* __M__ Component lifecycle hooks overview
	* __M__ Lifecycle sequence
	* __M__ Interfaces are optional (technically)
	* __H__ Other Angular lifecycle hooks
	* __A__ Lifecycle examples
	* __A__ Peek-a-boo: all hooks
	* __A__ Spying OnInit and OnDestroy
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
	* __A__ Pass data from parent to child with input binding
	* __M__ Intercept input property changes with a setter
	* __A__ Intercept input property changes with ngOnChanges()
		* _Previous section on OnChanges covers what  needs* to be covered, this just gives a little more detail_
	* Parent listeners for child event
		* _Previous section on Input and Output properties* covers enough of this, this just gives more detail_
	* __M__ Parent interacts with child via local variable
	* __M__ Parent calls an @ViewChild()
	* __M__ Parent and children communicate via a service
*__M__ __D__  Component Styles
	* __M__ __D__ Using component styles
	* __M__ __D__ Style scope
	* __M__ __D__ Special selectors
		* __M__ __D__ :host
		* __M__ __D__ :host-context
	* __M__ __D__ Loading component styles
		* __M__ __D__ Styles in component metadata
		* __M__ __D__ Style files in component metadata
		* __M__ __D__ Template inline styles
		* __M__ __D__ Template link tags
		* __M__ __D__ CSS @imports
		* __M__ __D__ External and global style files
		* __M__ __D__ Non-CSS style files
	* __M__ __D__ View encapsulation
	* __M__ __D__ Inspecting generated CSS
* __A__ Dynamic Components
	* __A__ Dynamic component loading
	* __A__ The anchor directive
	* __A__ Loading components
	* __A__ Resolving components
	* __A__ The AdComponent interface
	* __A__ Final ad banner
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
	* __A__ Power Boost Calculator
	* __A__ Pipes and change detection
	* __A__ Pure and impure pipes
	* Next steps
	* __M__ Appendix: No FilterPipe or OrderByPipe
* __A__ Animations
	* __A__ Overview
	* __A__ Setup
	* __A__ Transitioning between two states
	* __A__ States and transitions
		* __A__ The wildcard state *
		* __A__ The void state
	* __A__ Example: Entering and leaving
	* __A__ Example: Entering and leaving from different states
	* __A__ Animatable properties and units
	* __A__ Automatic property calculation
	* __A__ Animation timing
		* __A__ Duration
		* __A__ Delay
		* __A__ Easing
		* __A__ Example
	* __A__ Multi-step animations with keyframes
	* __A__ Parallel animation groups
	* __A__ Animation callbacks
## Forms
* __M__ User Input
	* Binding to user input events
	* __M__ Get user input from the $event object
		* __M__ Type the $event
		* __M__ Passing $event is a dubious practice
	* __A__ Get user input from a template reference variable
	* __M__ Key event filtering (with key.enter)
	* On blur
	* __H__ Put it all together
		* __H__ Observations
	* Source code
	* Summary
* __W__ Template-driven Forms
* __W__ Reactive Forms
* __W__ Dynamic Forms
## Bootstrapping
* __M__ The declarations array
	* __M__ Using directives with @NgModule
* __M__ The imports array
* __M__ The providers array
* __M__ The bootstrap array
* __M__ More about Angular modules
## NgModules
* __H__ NgModules introduction
	* __H__ Angular Modularity
	* __H__ The basic NgModule
	* __H__ More on NgModules
* __M__ JS Modules vs NgModules
	* __M__ JavaScript modules
	* __M__ NgModules
	* __M__ More on NgModules
* __M__ Frequently Used NgModules
	* __M__ Importing modules
	* __M__ BrowserModule and CommonModule
	* __M__ More on NgModules
* __A__ Types of NgModules
	* __A__ More on NgModules
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
	* __A__ Limiting provider scope by lazy loading modules
	* __A__ Limiting provider scope with components
	* __A__ Providing services in modules vs. components
	* __H__ More on NgModules
* __A__ Singleton Services
	* __A__ Providing a singleton service
	* __A__ forRoot()
	* __A__ Prevent reimport of the CoreModule
	* __A__ More on NgModules
* __A__ Lazy Loading Feature Modules
	* __A__ High level view
	* __A__ Set up an app
	* __A__ __W__ Create a feature module with routing
	* __A__ Add a component to the feature module
	* __A__ Add another feature module
	* __A__ Set up the UI
	* __A__ Configure the routes
		* __A__ Routes at the app level
		* __A__ Inside the feature module
		* __A__ Configure the feature module's routes
	* __A__ Confirm it's working
	* __A__ forRoot() and forChild()
	* __A__ More on NgModules and routing
* __M__ Sharing NgModules
	* __M__ Using components vs services from other modules
	* __M__ More on NgModules
* __H__ NgModules API
		__H__ Purpose of @NgModule
		__H__ @NgModule metadata
		__H__ More on NgModules
* __H__ NgModule FAQs
## Dependency Injection
* __H__ The Dependency Injection pattern
	* __H__ Why Dependency Injection
* __H__ Angular Dependency Injection
	* _This topic seems to already be covered quite a bit in the other material, so this section is optional_
	* __H__ DI by example
	* __H__ Create an injectable HeroService
	* __H__ Register a service provider
		* __H__ @Component providers
		* __H__ @NgModule providers
		* __H__ @NgModule or @Component
	* __H__ Inject a service
	* __H__ Singleton services
	* __H__ Component child injectors
	* __H__ Testing the component
	* __H__ When the service needs a service
	* __H__ @Injectable()
	* __H__ Providers 
		* __H__ The class as its own provider
		* __H__ The provide object
		* __H__ Alternative class providers
		* __H__ Class provider with dependencies
		* __H__ Aliased class providers
		* __H__ Value providers
		* __H__ Factory providers
	* __H__ Dependency Injection tokens
		* __H__ Non-class dependencies
		* __H__ TypeScript interfaces aren't valid tokens
		* __H__ Injection Token
	* __H__ Optional dependencies
	* __H__ Summary
* __A__ Hierarchical Injectors
	* __A__ The injector tree
		* __A__ Injector bubbling
		* __A__ Re-providing a service at different levels
	* __A__ Component injectors
		* __A__ Scenario: service isolation
		* __A__ Scenario: multiple edit sessions
		* __A__ Scenario: specialized providers
* DI in Action
	* __M__ Application-wide dependencies
	* __M__ External module configuration
	* __M__ @Injectable() and nested service dependencies
		* __M__ @Injectable()
	* __M__ Limit service scope to a component subtree
		* __M__ Take a break!
	* __A__ Multiple service instances (sandboxing)
	* __A__ Qualify dependency lookup with @Optional() and @Host()
		* __A__ Demonstration
	* __A__ Inject the components DOM element
	* __A__ Define dependencies with providers
		* __A__ Defining providers
	* __A__ Provider token alternatives: the class-interface and* injection token
		* __A__ Class-interface
		* __A__ InjecctionToken
	* __A__ Inject into a derived class
	* __A__ Find a parent component by injection
		* __A__ Find a parent component of known type
		* __A__ Cannot find a parent its base class
		* __A__ Find a parent by its class-interface
		* __A__ Find the parent in a tree of parents with @SkipSelf()
		* __A__ The Parent class-interface
		* __A__ A provideParent() helper function
	* __A__ Break circulatories with a forward class reference (forwardRef)
## HttpClient
* __M__ Setup: installing the module
* __M__ Making a request for JSON data
	* __M__ Typechecking the response
	* __M__ Reading the full response
	* __M__ Error Handling
	* __M__ Requesting non-JSON data
* __A__ Sending data to the server
	* __A__ Making a POST request
	* __A__ Configuring other parts of the request
* __A__ Advanced Usage
	* __A__ Intercepting all requests or responses
	* __A__ Listening to progress events
* __A__ Security: XSRF protection
	* __A__ Configuring custom cookie/header names
* __A__ Testing HTTP requests
	* __A__ Mocking philosophy 
	* __A__ Setup
	* __A__ Expecting and Answering requests
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
* __H__ The sample application
	* __H__ The sample application in action
* __H__ Milestone 1: Getting started with the router
	* __H__ Set the <base href>
	* __H__ Importing from the router library
	* __H__ The AppComponent shell
	* __H__ RouterOutlet
	* __H__ RouterLink binding
	* __H__ RouterLinkActive binding
	* __H__ Router directives
	* __H__ Wildcard route
	* __H__ The default route to heroes
	* __M__ Redirecting routes
	* __H__ Basics wrap up
* __H__ Milestone 2: Routing module
	* __H__ Refactor the routing configuration into a routing module
	* __H__ Do you need a Routing Module?
* __H__ Milestone 3: Heroes feature
	* __H__ Add heroes functionality
	* __H__ Hero feature routing configuration
	* __H__ Add the routing module to the HeroesModule
	* __H__ Remove duplicate hero routes
	* __H__ Import hero module into AppModule
	* __M__ Module import order matters
	* __M__ Route definition with a parameter
	* __M__ Setting the route parameters in the list view
	* __H__ ActivatedRoute in action
	* __H__ Navigating back to the list component
	* __H__ Route Parameters: Required or optional?
	* __H__ Heroes list: optionally selecting a hero
	* __H__ Route parameters in the ActivatedRoute service
	* __A__ Adding animations to the routed component 
	* __H__ Milestone 3 wrap up
* __H__ Milestone 4: Crisis center feature
	* __H__ A crisis center with child routes
	* __H__ Child routing component
	* __M__ Child route configuration
	* __H__ Import crisis center module into the AppModule routes
	* __M__ Relative navigation
	* __H__ Navigate to crisis list with a relative URL
	* __H__ Displaying multiple routes in names outlets
* __A__ __W__ Milestone 5: Route guards
	* __A__ __W__ CanActivate: requiring authentication
	* __A__ __W__ Component-less route: grouping routes without a component
	* __A__ __W__ CanActivateChild: guarding child routes
	* __A__ __W__ CanDeactivate: handling unsaved changes
	* __A__ __W__ Cancel and save
	* __A__ __W__ Resolve: pre-fetching component data
	* __A__ __W__ Fetch data before navigating
	* __A__ __W__ Query parameters and fragments
* __A__ __W__ Milestone 6: Asynchronous routing
	* __A__ __W__ Lazy loading route configurations
	* __A__ __W__ CanLoad guard: guarding unauthorized loading of feature modules
	* __A__ __W__ Preloading: background loading of feature areas
	* __A__ __W__ Custom Preloading Strategy
* __M__ Migrating URLs with Redirects
	* __M__ Changing /heroes to /superheroes
* Inspect the router's configuration
* Wrap up and final app 
## __H__ Cheat Sheet
