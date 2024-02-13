 Inline styling
mandatory
Copy over the task_5 directory from the 0x04. React components project (We’ll be using it as the base for this project)
Rename the task_5 directory to task_0
Modify the CourseListRow component in task_0/dashboard/src/CourseList/CourseListRow.js:

Using inline styling, change the background color of a row to #f5f5f5ab
Using inline styling, change the background color of a header row to #deb5b545
If needed, modify the test file so every test pass
Tips:

For better performances, never create and pass an object to an element directly. Use a constant instead
Use the isHeader prop to easily pick the style you want to apply to the tr tag
Requirement:

Even if the modification is small, make sure that your test suites are still passing. Especially the file CourseListRow.test.js
Repo:

GitHub repository: alx-react
Directory: 0x04-React_inline_styling
File: task_0/dashboard/src/CourseList/CourseListRow.js, task_0/dashboard/src/CourseList/CourseListRow.test.js
  
1. install Aphrodite
mandatory
Install Aphrodite using npm with:

npm install --save aphrodite

Modify the App component in task_1/dashboard/src/App/App.js:

Modify the component to use Aphrodite within the js file
Define the styling for the body and the footer within the file
Delete the file App.css and the import
Modify the BodySectionWithMarginBottom component in task_1/dashboard/src/BodySection/BodySectionWithMarginBottom.js:

Modify the component to use Aphrodite within the js file
Define the styling for the margin within the file
Delete the file BodySection.css and the import
Modify the CourseList component in task_1/dashboard/src/CourseList/CourseList.js:

Modify the component to use Aphrodite within the js file
Define the styling for the list within the file
Remove the styling for the list within the CourseList.css file
Modify the Header component in task_1/dashboard/src/Header/Header.js:

Modify the component to use Aphrodite within the js file
Define the styling for the logo and the header within the file
Delete the file Header.css and the import
Modify the Login component in task_1/dashboard/src/Login/Login.js:

Modify the component to use Aphrodite within the js file
Define the styling for the margin within the file
Delete the file Login.css and the import
Modify the Notifications component in task_1/dashboard/src/Notifications/Notifications.js:

Modify the component to use Aphrodite within the js file
Define the styling for the notifications panel within the file
Remove the styling for the notifications panel from the Notifications.css
Make sure the test suites are still passing!

Tips:

Look into using StyleSheetTestUtils.suppressStyleInjection at the top of your test file, to prevent issues with style injections
Requirements:

At this point, the UI should look exactly the same with the inline styling as it was with the CSS files
Repo:

GitHub repository: alx-react
Directory: 0x04-React_inline_styling
File: task_1/dashboard/src/App/App.js, task_1/dashboard/src/BodySection/BodySectionWithMarginBottom.js, task_1/dashboard/src/CourseList/CourseList.js, task_1/dashboard/src/Header/Header.js, task_1/dashboard/src/Login/Login.js, task_1/dashboard/src/Notifications/Notifications.js, task_1/dashboard/src/App/App.test.js,task_1/dashboard/src/BodySection/BodySectionWithMarginBottom.test.js, task_1/dashboard/src/CourseList/CourseList.test.js, task_1/dashboard/src/Header/Header.test.js, task_1/dashboard/src/Login/Login.test.js, task_1/dashboard/src/Notifications/Notifications.test.js
  
2. Conditionally applying style
mandatory
Modify the NotificationItem component in task_2/dashboard/src/Notifications/NotificationItem.js:

Modify the component to use Aphrodite within the js file
Define the styling for the urgent and default items
Using condition, apply the styling to the li element
Delete the Notifications.css file and remove any import
Modify the NotificationItem.test suite in task_2/dashboard/src/Notifications/NotificationItem.test.js:

Make sure that tests are still passing
Modify the CourseListRow component in task_2/dashboard/src/CourseList/CourseListRow.js:

Modify the component to use Aphrodite within the js file
Define the styling for the different type of rows (default rows, header rows)
Define the styling for the different type of th elements
Delete the CourseList.css file and remove any import
Modify the CourseListRow.test suite in task_2/dashboard/src/CourseList/CourseListRow.test.js:

Make sure that tests are still passing
Test properties one by one if easier
Requirements:

Use conditions as much as you can, do not repeat elements
At this point, the UI should look exactly the same with the inline styling as it was with the CSS files
Tips:

You can either use conditions or use an array to apply the different styling. Conditions are usually more robust
Testing might become difficult with the different variations. Look into the Enzyme documentation for render, contains, prop, and html
Repo:

GitHub repository: alx-react
Directory: 0x04-React_inline_styling
File: task_2/dashboard/src/Notifications/NotificationItem.js, task_2/dashboard/src/Notifications/NotificationItem.test.js, task_2/dashboard/src/CourseList/CourseListRow.js, task_2/dashboard/src/CourseList/CourseListRow.test.js
  
3. Responsive design
mandatory
Let’s make the application responsive to the screen size using media queries. We are going to only focus on large screen and screens with a width under 900px

Modify the component Login in task_3/dashboard/src/Login/Login.js:

Make sure that a label and an input are on each line
Make sure that the button is on a new line
The screen should look like the image below:


Modify the component Notifications in task_3/dashboard/src/Notifications/Notifications.js:

When the panel is open, it should take over the entire screen
There should be no padding because of the ul element
The font size of the text should be 20px
Modify the component NotificationItem in task_3/dashboard/src/Notifications/NotificationItem.js:

The item should take the entire screen width
A black border should be displayed at the bottom
The font size of the text should be 20px
The padding for the item should be 10px 8px
Requirements:

When the notifications panel is open, the screen should look like the image below:


Repo:

GitHub repository: alx-react
Directory: 0x04-React_inline_styling
File: task_3/dashboard/src/Login/Login.js, task_3/dashboard/src/Notifications/Notifications.js, task_3/dashboard/src/Notifications/NotificationItem.js
 
4. Animation
mandatory
Let’s create an animation that we can display when the user hovers on the Notifications menu or when there is a new notification. In task_4/dashboard/Notifications/Notifications.js:

Create one object containing the CSS frames to make the opacity change from 0.5 to 1
Create one object containing the CSS frames to make the element bounce. You can play with translateY and alternate from 0px to -5px and 5px
Modify the styling for the menu item to:

Float on the right of the screen over every element
The background color should be #fff8f8
Show the pointer cursor when hovering the element
On hover, animate the element with the two new animations. The duration for the opacity change should be 1s, and the duration for the bouncing effect should be 0.5s. The animation should repeat 3 times only
When the list of notifications is visible, hide the menu item
Requirements:

When the notifications panel is hovered or opened, the UI should look like the image below:


Repo:

GitHub repository: alx-react
Directory: 0x04-React_inline_styling
File: task_4/dashboard/src/Notifications/Notifications.js

About
Inline styles are great for distributed react components via npm or just reusable components in general. Having everything you need to run the component requirable within javascript improves its usability greatly. Having to look for an external css file in the node_modules folder sucks.

However using inline styles, we quickly run into multiple problems. The main one being the missing possibility to adjust styles from outside the component but also the missing pseudo classes (mainly :hover) and media queries can sometimes be really handy and are duly missed. And while these last two can be substituted with javascript, there are situations where global css is needed (think: HTML API responses, 3rd party plugins etc).

There is a lot of discussion going on about these problems and the missing modularity of css in general.
Check out @Vjeux on CSS in JS as a good starting point.

React Inline Style focuses on reusable, self contained components, that dont require any external css file but are still adaptable and styleable by their owner / end user / developer.

Features
React Inline Style provides a practical solution for the following problems:

Define ALL styles in JavaScript within the component/module.
Owner component can influence/override its child components styles.
Define global css rules and media-queries also from within a component.
Easy substitution for conditional class definitions like :hover and :pressed.
What React Inline Style does not provide:

Export styles into global stylesheet.
Basic Usage
React Inline Style is used as react mixin.
Styles can be defined with the define() methods and are applied through the style property with the this.style() method.

var React = require("react");
var Style = require("react-inline-style");

Style = Style.define({  //                           <-- make sure to redefine Style with the output of Style.define()
  textComponent : {
    fontWeight:"bold",
    fontStyle:"italic"
  }
});
 
var TextComponent = React.createClass({
  
  mixins : [Style()],  //                           <-- make sure to include the mixin              

  click : function(){
    this.style.define({
      textComponent : {
        fontStyle:"normal",
        letterSpacing:"2px"
      }
    });
    this.forceUpdate();
  },

  render : function (){
    return (
      <p 
        style={this.style("textComponent")} 
        onClick = {this.click}>
          textComponent
      </p>
    );
  }

});

React.render(<TextComponent />, document.body);
Demo: jsFiddle

Style Definition
Styles can be defined on a module-level or the instance-level of the component.

var React = require("react");
var Style = require("react-inline-style");

Style = Style.define({...}); //             <-- module-level
 
React.createClass({
  mixins : [Style()],
  render : function (){
    
    this.style.define({...}); //            <-- instance-level
  
    [...]
  }
});
Styles defined on module-level will apply to all instances of the component (Think: Static styles) while instance-level styles only apply to the current instance/placement (Think: Dynamic styles).

Both define() methods take the same parameters. See API: Style.define(); for more info.

Style Application
Styles are applied through the style property with the this.style() method.

this.style() takes either "class names" whos definitions can be modified and overridden by parent/owner components, or style definitions as object literals. The later cant be overridden from the outside.

Styles passed to this.style() are applied/override each other in the order they were passed in.

var React = require("react");
var Style = require("react-inline-style");

Style = Style.define({
  myStyle : {
    fontWeight:"bold",
    color:"blue"
  }
});
 
React.createClass({
  mixins : [Style()],
  render : function (){
    return (<p style={this.style("myStyle", {color:"red"})}>textComponent</p>); 
  }
});
Demo: jsFiddle

Inheritance
Defined styles are passed down the component tree and override its child components style definitions. This makes it possible to adjust and influence components without changing their code.

The inheritance also works through RandomComponents that do neither use nor include the react-inline-style mixin.

var React = require("react");
var Style = require("react-inline-style");

var TextComponent = require("./TextComponent"); // See definition in "Basic Usage".
var RandomComponent = require("RandomComponent"); // This can be any component.

Style = Style.define({
  textComponent : {
    color : "red"
  }
});
 
var RootComponent = React.createClass({
  
  mixins : [Style()],

  render : function (){
    return (
      <RandomComponent> 
       <TextComponent \>
      </RandomComponent>
    );
  }

});

React.render(<RootComponent />, document.body);
Demo: jsFiddle

Namespaces / Nesting Styles
Namespacing is super useful and even necessary when using modular css.

There are two ways of namespacing a component with React Inline Style:

Namespaceing from inside a component
Within your component you can nest your style definitions in order to create namespaces:

Style.define({

  myNamespace : {
    textComponent : {
      color :"red"
    }
  }
});

// available through

this.style("myNamespace.textComponent")
And namespaces can also be passed in as the first parameter:

Style.define("myNamespace.textComponent", {
    color :"red"
});

// also available through

this.style("myNamespace.textComponent")
styleNamespace Property (Namespacing from outside a component)
When using multiple components within one parent component, namespace collisions can happen and styles can't be defined for a particular component alone.

To prevent this you can use the property styleNamespace to define a namespace for this component instance from the ouside:

var React = require("react");
var Style = require("react-inline-style");

var TextComponent = require("./TextComponent"); // See definition in "Basic Usage".

Style = Style.define({
  first : {
    textComponent : {
      color : "red"
    }
  },
  second : {
    textComponent : {
      color : "blue"
    }
  }
});
 
var RootComponent = React.createClass({
  
  mixins : [Style()],

  render : function (){
    return (
     <TextComponent styleNamespace = "first" \>
     <TextComponent styleNamespace = "second" \>
    );
  }

});

React.render(<RootComponent />, document.body);
Demo: jsFiddle

Global Styles
In some situations global styles are necessary (3rd party html) in others they are useful or improve performance (media queries).

React inline style provides the possibility to define global styles from within a component through Style.global(). Style definitions passed to Style.global() are transformed to normal css definitions and are added to the document <head>.

Style.global({
  ".example" : {
    color : "red",
  
    "p, a" : {
      fontWeight:"bold"
    }
  },
  
  "@media (max-width: 600px)":{
    ".example" : {
      color:"blue"
    }
  }
});


// Becomes in <head /> 

<style id="mgy3joepeffuhaor" class="react-inline-style global-css">
  
  .example {
    color:"red";
  }
  
  .example p {
    font-weight:bold;
  }
    
  .example a {
    font-weight:bold;
  }
  
  @media (max-width: 600px) {
    .example {
      color:"blue";
    }
  }

</style>
Style.global() only exists on module-level. Although it can be updated at any time on instance-level. these styles are global and affect all instances.

Conditionals / :pseudo classes
Using inline styles, :pseudo classes are not available. However they can be substitued easily with react's this.state.

Doing so, often requires tests like this.state.hover && "hoverStyle" to apply hoverStyle only if this.state.hover is actually true.

React Inline Style makes this easier by reintroducing :pseudo classes. When applying a style class through this.style(), you can add any pseudo :variableName to it. Doing so results in a check for this.state.variableName and the styles are only applied if it returned true:

"hoverStyle:hover"    ===  this.state.hover && "hoverStyle"

"hoverStyle:myState"  ===  this.state.myState && "hoverStyle"
Also the two most common :pseudo classes :hover and :pressed are already implemented for you. Just use them and all the required event handlers will be attached once their needed and removed when their not. (Still no solution for :focus though)

Demo: jsFiddle

Extend Style Classes
Style definitions can _extend other styles.

Style.define({
  defaults : {
    myStyle : {
      color:"blue",
      fontWeight: "bold" 
    }
  },
  myStyle : {
    
    _extend:"defaults.myStyle",
    
    color:"red"
  }
});
this.style("myStyle") now results in:

{ color:"red", fontWeight:"bold" }; 
API
React Inline Style is a React mixin. Make sure to include it into your component:

  Style = require("react-inline-style");

  React.createClass({
    mixins : [Style()],
    ...
  });
  
Style.define( [ namespace, ] styles);
RETURNS function: New Style instance.
Defines styles on module-level

namespace optional

TYPE string / array

Onle or multiple namespaces to encapsulate this definition

["namespace", "another.namespace"]

or 

"namespace, another.namespace"
styles required

TYPE object

Style definitions

{
  styleClass : {
    color: "red",
    backgroundColor:"red",
   
    nestedStyle : {
      fontWeight: "bold"    
    }
  },
  anotherStyle: {
    _extend : "styleClass.nestedStyle",
    color: "purple"
  }
}
See Style Definition for more info.

Style.global( [ namespace, ] styles);
RETURNS function: New Style instance.
Defines global styles that will be placed in <head>

namespace optional

TYPE string / array

Onle or multiple namespaces to encapsulate this definition

[".namespace", ".another .namespace"]

or 

".namespace, .another .namespace"
styles required

TYPE object

Style definitions:

{
  ".styleClass" : {
    color: "red",
    backgroundColor:"red",
    ...
    ".nestedStyle" : {
      fontWeight: "bold"    
    }
  },
  ".anotherStyle": {
    color: "purple"
  }
}
See Global Styles for more info.

this.style([ styleClass, ][ styleDefinition, ][ styleGroup, ]);
RETURNS object: Style definition.
Takes any number of parameters/styles and combines them to one valid style definition that can be passed to the style property.
Style definitions override each other in the order they were passed into the function.

styleClass optional

TYPE string

StyleClass string.

"myStyle"
"namespace.myStyle"
"namespace.myStyle:hover"
"myStyle:conditional"
styleDefinition optional

TYPE object

Style definitions

{
  color: "red",
  backgroundColor: "white",
  fontWeight: "bold",
  fontStyle: "italic",
}
styleGroup optional

TYPE array

A collection of styleClasses, styleDefinitions and styleGroups

[ "myStyle", "namespace.myStyle:hover", {color:"red"} ]
See Style Application for more info.

this.style.define( [ namespace, ] styles);
RETURNS null
Defines styles on instance-level

namespace optional

TYPE string / array

Onle or multiple namespaces to encapsulate this definition

["namespace", "another.namespace"]

or 

"namespace, another.namespace"
styles required

TYPE object

Style definitions

{
  styleClass : {
    color: "red",
    backgroundColor:"red",
    
    nestedStyle : {
      fontWeight: "bold"    
    }
  },
  anotherStyle: {
    _extend : "styleClass.nestedStyle",
    color: "purple"
  }
}
See Style Definition for more info.

this.style.log();
RETURNS null
Logs the current "virtual stylesheet" and namespace into the console

License
License: MIT

Released in 2015 by Philipp Adrian @ Dow Jones
