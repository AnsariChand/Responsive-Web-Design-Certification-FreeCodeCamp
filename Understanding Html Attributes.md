# What Role Does Html Play on the Web?

## What is Html?

Html, which Stands for HyperText Markup Language, is a markup language for creating web pages. When you visit a Website and see content like paragraphs, heading, links, images, and Videos, that's HTML.

Here is a Small example using Html elements. Try editing some of the text in the Editor and see the changes update in the preview window.

```
<h1> Main heading element </h1>
<P> I am a Paragraph element. </P>
```

Html Represents the content and Structure of a Webpage through the use of elements. Most elements will have an opening tag and closing tag. Sometimes those tags are referred to as start and end tags. In between those two tags, you will have the content. This content can be text or other HTML elements.

Here is another example of a Paragraph element. Change the text in the editor to say I Love Coding! and see the results in the preview window.

```
<p> I am a Paragraph element. </p>
```

## Opening and Closing Tags

Both opening and closing tags starts with a left angle bracket (<), and end with a right angle bracket (>), with the tag name placed between these angle brackets. While HTML tag names are case-insensitive, it is a widely accepted convention and best practice to write them in lowercase.

Here is Closer look at just the opening and closing paragraph tag:

```
<P> </P>
```

What distinguishes an opening tag from a closing tag is the forward slash (/) placed immediately after the left angle bracket in a closing Tag. Some Html elements do not have a closing tag. These are Known as Void elements.

## Void Elements

Here is an Example of an image element which is a void element:

```
<img>
```

Notice that this image element does not have the closing tag and it does not have any content. Void elements cannot have any content and only have a Start tag.

Sometimes you will see void elements that use a [ / ] before the [ > ] like this:

```
</img>
```

While many code formatters like Prettier will choose to include the [ / ] in void elements, the Html spec states that the presence of the [ / ] "does not mark tag as self-closing but instead is unnecessary and has no effect of any kind".

In Real-worls development, you will see both forms, so it is important to be familiar with both.

## HTML Attributes

If You want to display an image, you will need to include a couple of Attributes inside your image element. An attribute is a special value used to adjust the behavior of an Html element.

Here is an Example of an image element with a Src attribute. Update the value of the Src attribute to
"https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" and you will see the image change to two cats peacefully sleeping.

```
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg"/>
```

The Src attribute is used to specify the location for that image. For image elements, it's good practice to include another attribute called the alt attribute. the alt attribute is used to provide short, descriptive text for the images.

Here's an example of an image element with the src and alt attributes. Try breaking the image by updating the Src value to "https://.freecodecamp.org/curriculum/cat-photo-app/cat.jpg". You will see the image disappear and only the alt text show.

```
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Two tabby kittens sleeping together on a couch.">
```

## Html's Role Alongside CSS and JavaScript

So, you might be wondering if HTML by itself is enough to build a Website. well, the answer is: it depends. if you're building a small practice project that onlu display text and images, Html alone might be sufficient. However, if you're creating a modern professional website, you will need to have HTML, CSS and JavaScript.

HTML is for the content and Structure. CSS is for Styling. javaScript is for adding interactivity to your web pages. A good analogy for this is to compare HTML, CSS, and JavaScript with a complete building.

HTML represents the blocks, concrete, and irom that make up the walls. it`s the foundation that makes the building strong.
CSS represents the interior and exterior design that makes the building look beautiful. Javascript represents the electrical and water system that ensures uninterrupted acces to water and electricity.

**Quesitions:**
Q:1 What does HTML stand for?

- HyperText Markup Language

Q:2 Which is the following is the correct syntax for a closing Tag?

```
- <;p>
- </p>
- <p>
- <///p/>

<!-- </p> -->
```

Q:3 Which if the following is a Valid attribute used inside the img element?

```
- Src
- bold
- Closing
- div
<!-- Src -->
```

# What are Attributes, and How Do They Work?

## What Is an Attribute?

An attribute ia a Value placed inside the opening tag of an HTML element. Attributes provide additional information about the element or specify how the element should behave. Here is the basic syntax for an attribute:

```
<element attribute="value"> </element>
```

The attribute name is followed by an equal sign ( = ) and a value in quotes. The value can be a String or a number, depending on the attribute.

## The **href** and **Target** Attributes

This first example uses the _href_ and _target_ attributes. the href attribute specifies the URL of a link and the target attribute specifies where to open the link.

**NOTE:** The _a_ element, also known as the anchor element, is use to create hyperlinks. The text between the opening and closing a Tags is the clickable part users selcet to navigate.

Enable the interactive editor and change the href="https://www.freecodecamp.org/news/" to

href="https://www.freecodecamp.org".
Now when you click on the link in the interactive editor, you will see the freecodecamp homepage in a new browser tab.

```
<a href="https://www.freecodecamp.org/news/" target="_blank"> Visit freeCodeCamp</a>
```

Without the href attribute, the link would not work because there would be no destincation URL. so you must include this _href_ attribute to make the link functional. The target="\_blank" enables the link to open in a new browser tab. you will learn more about the _target_ attribute in future lessons.

## The Src and alt Attributes

Other common attributes are the Src and alt, or alternative, attributes, which are used to specify the source of an image and provide alternative descriptiove text for the image, respectively.

Enable the interactive editor and change the src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" to src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg". Then change the alt="Two tabby kittens sleeping together on a couch." to alt="Two cats running in the dirt.".

```
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Two tabby kittens sleeping together on a couch. " />
```

Similar to the _href_ attribute, the _src_ attribute is required because it specifies the image file to be displayed. The _alt_ attribute is not required, but it is recommended for accessibility purposes.

Accessibility means making sure that everyone, including those with disabilities, can use and undesrstand things like websites, apps, and physical spaces. you will learn more about accessibility in the upcoming lessons.

## The Checked Attribute

Some Attributes are a little unique with their syntax like the checked attribute.

Enable the interactive editor and try clicling on the checkbox in the preview window to see it alternate between a checked and unchecked state.

```
<input type="checkbox" checked />
```

In the following example, we have an _input_ element with the _type_ attribute set to _checkbox_. Inputs are used to collect data from users, and the type attributes specifies the type of input. In this case, this input is a checkbox. You will learn more about how inputs work in the upcoming lessons.

The _Checked_ attribute is used to specify that the checkbox should be checked by default. The _checked_ attributes does not require a value.if it is present, the checkbox will be checked by default. if the attribute is not present, the checkbox will be unchecked. This is Known as a boolean attribute. you will learn more about booleans in general when you get to the javaScript section.

Enable the interactive editor and try removing the _checked_ attribute from the _input_. You will see that the checkbox is no longer checked by default.

```
<input type="checkbox" checked />
```

## Other Boolean Attributes

There are several common boolean attributes you will encounter in Html, such as _disabled_, _readonly_, and _required._
These attributes are used to specify the state of an element, such as whether it is disabled, read-only, or required.

Here is an Example of a text _input_ element that is disabled by default. Enable the interactive editor and try clicking on the _input_ element in the preview window.
Now remove the _disabled_ attribute from the _input_ element and you will see that the _input_ is no longer disabled by default.
You should now be able to click on it and type inside the field.

```
<input type="text" disabled>
```

HTML has many attributes that can be used to customize the behavior and appearance of elements on a Webpage. Understanding how to use attributes is essential for creating interactive and accessible web content. Over the Next few lessons, you will learn about more Html attributes and how to use them effectively in your web development projects.

-------Question--------
Qus: Which of the Following is an Example of a Boolean attribute?

```
- Src
- href
- disabled
- alt
<!--  disabled -->
```

Qus: What is the role of an attribute in HTML?

```
- Attributes provide additional information and help define the behavior for HTML elements.

- Attribute change the background color of an element.

- Attributes change the font size of an element.

- Attributes add javaScript functionality to an element.

<!-- Attributes provide additional information and help define the behavior for HTML elements. -->
```

Qus: Which of the following is the correct syntax for a boolean attribute?

```
<input type="checkbox" checked>
<input type="checkbox" checked="on">
<input type="checkbox" checked="off">
<input type="checkbox" checked="isChecked">
<!-- <input type="checkbox" checked>
  -->
```
