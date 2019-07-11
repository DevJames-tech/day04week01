# week1Day4-Person


Android Manifest:

Design Patterns:


Singleton Design Pattern :

is a guideline on the best way to create an object .
The pattern uses a Singular Class whose job is to make sure only 1 singular object is created at a time. Also it provides a shortcut which allows you to access this object without creating an object of a class first.

￼
 Factory Design Pattern:

Is one of the most used patterns in java. It focuses on abstracting the logic from the client protecting the creation logic of the object.

￼

Builder Design Pattern:
Builds a complex object by combining other Simplier objects, this is another Pattern for the creation of an object

￼

 Facade Design Pattern:
Falls under the category of being a structural Design pattern. It abstract the complexity of the System, behind a user friendly client interface. Allowing the client to manipulate the system.

￼

 Prototype Design Pattern:
Is pattern that gives you a way to clone an object instead of doing costly operations to build a new one.

￼



Android Runtime (ART):

is the managed runtime used by applications and some system services on Android. Uses Ahead-of Time (AOT) compilation, I.e. translate high-level languages into machine code. So it can compile natively.

These allow much longer battery life for androids, along with better memory management and less memory usage. The biggest downside is that the first time you compile, it will be significantly longer the first time around


Dalvik:
Is a virtual machine that android runs on and also runs anything from applications to code written in the java language

Java code is transcoded into Byte code which then converted into a .dex file which the Dalvik VM can read and use

Duplicate data used in class files is included only once in the .dex output, which saves space and uses less overhead. The executable files can be modified again when you install an application to make things even more optimized for mobile. Things like byte order swapping and linking data structure and function libraries inline make the files smaller and run better on our devices.


Refers to the Android Manifest File

This is an xml file which must be named as AndroidManifest.xml and placed at application root. Every Android app must have AndroidManifest.xml file. AndroidManifest.xml allows us to define,
The packages, API, libraries needed for the application.
* Basic building blocks of application like activities, services and etc.
* Details about permissions.
* Set of classes needed before launch.
Elements of AndroidManifest.xml
Following are the elements(listed alphabetically) that can appear in AndroidManifest.xml, this list is restricted and we cannot add our own elements to it.
<action>
<activity>
<activity-alias>
<application>
<category>
<data>
<grant-uri-permission>
<instrumentation>
<intent-filter>
<manifest>
<meta-data>
<permission>
<permission-group>
<permission-tree>
<provider>
<receiver>
<service>
<supports-screens>
<uses-configuration>
<uses-feature>
<uses-library>
<uses-permission>
<uses-sdk>
Elements for Application Properties
* uses-permission – used to specify permissions that are requested for the purpose of security.
* permission – used to set permissions to provide access control for some specific component of the application.
* permission-group – does the same as above for a set of components.
* permission-tree – refer one specific name of the component which is the owner or parent of the set of component.
* instrumentation – enables to know interaction between Android system and application.
* uses-sdk – specifies the platform compatibility of the application.
* uses-configuration – specifies set of hardware and software requirement of the application.
* uses-feature – specifies single hardware and software requirement and their related entity.
* supports-screens, compatible-screens – both these tags deals with screen configuration mode and size of the screen and etc.
* supports-gl-texture – specifies texture based on which the application is filtered.
Elements for Application Components
These should be enclosed in <application> container.
* activity – has the set of attributes based on user interface.
* activity-alias – specifies target activities.
* service – has the operation provided by any library or API, running in background that is not visible.
* receiver – that makes to receive message broadcasted by the same application or by outside entity.
* provider – provides some structure to access application data.
* uses-library – it specifies set of library files need to run the application.
These entire information has to be known by the system to run any file of the application. So that this file has to be created at the time of installing and not at the time of running the application.
If this is the second tutorial after Hello World, you may not be able to understand every element listed. Don’t worry, I just wanted to give an overview. As we progress we will understand about each of these in detail.
Structure of AndroidManifest.xml
<manifest>
<Elements for Application properties should come here - refer above for list>

<application>

<Elements for application components should come here - refere above for list>

</application>

</manifest>


View , View Group, View Hierachy 

View is anything can be view on android such as:
* Text View
* EditText
* Button
* ImageView
* ImageButton
* CheckBox
* Radio button
* RadioGroup
* ListView
* Spinner
* AutoCompleteTextView

A view group Holds and defines the properties of a view, View Group is the base class for layouts so their are interchangeable

View Hierarchy is the combination of view groups and their views. Resembles the tree data structure

￼


Constraint, Linear, Grid and Relative, Coordinator

Constraint:
Large and complex  layout with a flat view hierarchy(means no nested view groups)

Linear:
aligns all children in a single direction, vertically or horizontally.

Relative:
Displays child views in relative positions. The position of each view can be specified as relative to sibling elements (such as to the left-of or below another view) or in positions relative to the parent 

GridLayout:
A layout that places its children in a rectangular grid.
