# Object Literal
Object Literal. In plain English, an object literal is a comma-separated list of name-value pairs inside of curly braces. Those values can be properties and functions. Here's a snippet of an object literal with one property and one function.

# What is an object in JavaScript?
In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. A cup is an object, with properties. A cup has a color, a design, weight, a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics


# What is object and example?
An object can be a single-word noun (e.g., dog, goldfish, man), a pronoun (e.g., her, it, him), a noun phrase (e.g., the doggy in window, to eat our goldfish, a man about town), or a noun clause (e.g., what the dog saw, how the goldfish survived, why man triumphed)



![](https://www.grammar-monster.com/glossary/pics/object_grammar.png)



# What's the difference between subject and object?
As a basic rule: The subject is the person or thing doing something. The object is having something done to it.

# Objects overview
Objects in JavaScript, just as in many other programming languages, can be compared to objects in real life. The concept of objects in JavaScript can be understood with real life, tangible objects.

In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. A cup is an object, with properties. A cup has a color, a design, weight, a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics.

# Objects and properties
A JavaScript object has properties associated with it. A property of an object can be explained as a variable that is attached to the object. Object properties are basically the same as ordinary JavaScript variables, except for the attachment to objects. The properties of an object define the characteristics of the object. You access the properties of an object with a simple dot-notation:



for more detials please join the link:

[Object Literal](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects?retiredLocale=ar)


# What is the document object model in JavaScript?
The Document Object Model (DOM) is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. ... The DOM is an object-oriented representation of the web page, which can be modified with a scripting language such as JavaScript



# Document Object Model (DOM)
The Document Object Model (DOM) connects web pages to scripts or programming languages by representing the structure of a document—such as the HTML representing a web page—in memory. Usually it refers to JavaScript, even though modeling HTML, SVG, or XML documents as objects are not part of the core JavaScript language.

The DOM represents a document with a logical tree. Each branch of the tree ends in a node, and each node contains objects. DOM methods allow programmatic access to the tree. With them, you can change the document's structure, style, or content.

Nodes can also have event handlers attached to them. Once an event is triggered, the event handlers get executed.


![Document Object Model](https://simplesnippets.tech/wp-content/uploads/2018/10/what-is-document-object-model-in-JS-featured-image.jpg)


In the Document Object Model, documents have a logical structure which is very much like a tree; to be more precise, it is like a "forest" or "grove" which can contain more than one tree. However, the Document Object Model does not specify that documents be implemented as a tree or a grove , nor does it specify how the relationships among objects be implemented in any way. In other words, the object model specifies the logical model for the programming interface, and this logical model may be implemented in any way that a particular implementation finds convenient. In this specification, we use the term structure model to describe the tree-like representation of a document; we specifically avoid terms like "tree" or "grove" in order to avoid implying a particular implementation. One important property of DOM structure models is structural isomorphism: if any two Document Object Model implementations are used to create a representation of the same document, they will create the same structure model, with precisely the same objects and relationships.

The name "Document Object Model" was chosen because it is an "object model" is used in the traditional object oriented design sense: documents are modeled using objects, and the model encompasses not only the structure of a document, but also the behavior of a document and the objects of which it is composed. In other words, the nodes in the above diagram do not represent a data structure, they represent objects, which have functions and identity. As an object model, the Document Object Model identifies:

the interfaces and objects used to represent and manipulate a document
the semantics of these interfaces and objects - including both behavior and attributes
the relationships and collaborations among these interfaces and objects
The structure of SGML documents has traditionally been represented by an abstract data model, not by an object model. In an abstract data model, the model is centered around the data. In object oriented programming languages, the data itself is encapsulated in objects which hide the data, protecting it from direct external manipulation. The functions associated with these objects determine how the objects may be manipulated, and they are part of the object model.

The Document Object Model currently consists of two parts, DOM Core and DOM HTML. The DOM Core represents the functionality used for XML documents, and also serves as the basis for DOM HTML. All DOM implementations must support the interfaces listed as "fundamental" in the Core specification; in addition, XML implementations must support the interfaces listed as "extended" in the Core specification. The Level 1 DOM HTML specification defines additional functionality needed for HTML documents


# What the Document Object Model is not
This section is designed to give a more precise understanding of the Document Object Model by distinguishing it from other systems that may seem to be like it.

Although the Document Object Model was strongly influenced by Dynamic HTML, in Level 1, it does not implement all of Dynamic HTML. In particular, events have not yet been defined. Level 1 is designed to lay a firm foundation for this kind of functionality by providing a robust, flexible model of the document itself.
The Document Object Model is not a binary specification. Document Object Model programs written in the same language will be source code compatible across platforms, but the Document Object Model does not define any form of binary interoperability.
The Document Object Model is not a way of persisting objects to XML or HTML. Instead of specifying how objects may be represented in XML, the Document Object Model specifies how XML and HTML documents are represented as objects, so that they may be used in object oriented programs.
The Document Object Model is not a set of data structures, it is an object model that specifies interfaces. Although this document contains diagrams showing parent/child relationships, these are logical relationships defined by the programming interfaces, not representations of any particular internal data structures.
The Document Object Model does not define "the true inner semantics" of XML or HTML. The semantics of those languages are defined by the languages themselves. The Document Object Model is a programming model designed to respect these semantics. The Document Object Model does not have any ramifications for the way you write XML and HTML documents; any document that can be written in these languages can be represented in the Document Object Model.
The Document Object Model, despite its name, is not a competitor to the Component Object Model (COM). COM, like CORBA, is a language independent way to specify interfaces and objects; the Document Object Model is a set of interfaces and objects designed for managing HTML and XML documents. The DOM may be implemented using language-independent systems like COM or CORBA; it may also be implemented using language-specific bindings like the Java or ECMAScript bindings specified in this document.


for more details please join the link 

[Dom](https://www.w3schools.com/js/js_htmldom.asp)