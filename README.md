# CSS-Interview-Questions

## What is Cascade?

#### At a very simple level, cascade means that the order of CSS rules matter; when two rules apply that have equal specificity the one that comes last in the CSS is the one that will be used.

```
h1 {
    color: red;
}
h1 {
    color: blue;
}

<h1>This is blue heading.</h1>
```

## What is Specificity?

#### Specificity means how the browser decides which rule applies if multiple rules have different selectors, can still apply to the same element. It is basically a measure of how specific a selector's selection will be:

- An element selector is less specific — it will select all elements of that type that appear on a page — so will get a lower score.
- A class selector is more specific — it will select only the elements on a page that have a specific class attribute value — so will get a higher score.

```
.main-heading {
    color: red;
}

h1 {
    color: blue;
}

<h1 class="main-heading">This will be a red heading.</h1>
```

## What is Inheritance?

#### some CSS property values set on parent elements are inherited by their child elements, and some aren't. For example, if you set a color and font-family on an element, every element inside it will also be styled with that color and font, unless you've applied different color and font values directly to them.

```
body {
    color: blue;
}

span {
    color: black;
}
<p>As the body has been set to have a color of blue this is inherited through the descendants.</p>
<p>We can change the color by targetting the element with a selector, such as this <span>span</span>.</p>
```

- Some properties do not inherit — for example, if you set a width of 50% on an element, all of its descendants do not get a width of 50% of their parent's width. If this was the case, CSS would be very frustrating to use!

## What are the benefits of CSS sprites?

#### If a web page has a large number of images that take a longer time to load because each image separately sends out an HTTP request. The concept of CSS sprites is used to reduce the loading time for a web page because it combines the various small images into one image. It reduces the number of HTTP requests and hence the loading time.

## What is the CSS Box model and what are its elements?

#### The CSS box model is used to define the design and layout of elements of CSS. It describes the rectangular boxes that are generated for elements in the document tree and laid out according to the visual formatting model. Each box has a content area (e.g. text, an image, etc.) and an optional surrounding padding, border, and margin areas.

The elements are:

- Margin - It removes the area around the border. It is transparent.
- Border - It represents the area around the padding
- Padding - It removes the area around the content. It is transparent.
- Content - It represents the content like text, images, etc.

[Understand above three concepts together](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance#understanding_how_the_concepts_work_together)

## How to reset all the property of the element?

```
.[class-name] {
    all: unset;
}
```

## Shorthand properties?

#### Shorthand properties are CSS properties that let you set the values of multiple other CSS properties simultaneously. Using a shorthand property, you can write more concise (and often more readable) style sheets, saving time and energy. For example, background, margin, border, font, etc.

## What is the float property of CSS?

#### The float CSS property places an element on the left or right side of its container, allowing text and inline elements to wrap around it.

## What is the purpose of the z-index and how is it used?

#### The z-index helps to specify the stack order of positioned elements that may overlap one another. The z-index default value is zero and can take on either a positive or negative number.

## Explain the difference between visibility: hidden and display: none?

#### visibility: hidden hides the element, but it occupies space and affects the layout of the document. display: none also hides the element but not occupy space. It will not affect the layout of the document.

## What is tweening?

#### It is the process of generating intermediate frames between two images. It gives the impression that the first image has smoothly evolved into the second one. It is an important method used in all types of animations. In CSS3, Transforms (matrix, translate, rotate, scale) module can be used to achieve tweening.

## What is the difference between CSS2 and CSS3?

#### The main difference between CSS2 and CSS3 is that CSS3 is divided into different sections which are also known as modules. Unlike CSS2, CSS3 modules are supported by many browsers.Apart from that, CSS3 contains new General Sibling Combinators which is responsible for matching the sibling elements with the given elements.

## What is the meaning of cascading? How do style sheets cascade?

#### CSS brought about a revolution in web-development and how people perceive the process of building a website. Prior to the existence of CSS, elements had to be styled in an in-line fashion or the style were implemented in the head section of an HTML page. This was changed due to the cascading nature of CSS. Here are the three major ways CSS cascades:

- Elements – The same CSS style can be applied to multiple elements to achieve the same style.
- Multiple Style One Element – Multiple styles can be applied to a particular HTML element to achieve a unique style.
- Same style, Multiple Pages – The same stylesheet can be applied to different HTML pages altogether to achieve a template styling very quickly.

## What are the disadvantages of using CSS?

- Ascending by selectors is not possible
- Limitations of vertical control
- No expressions
- No Column declarations
- Pseudo-class not controlled by dynamic behaviour
- Rules, styles, targeting specific text not possible

## What are the ways to assign a certain colour to an element in CSS?

#### CSS can assign a wide range of colours to elements using different notations.

- Hexadecimal notation
- RGB functional notation
- HSL functional notation

## What are pseudo-elements in CSS?

#### A CSS pseudo-element is a keyword added to a selector that lets you style a specific part of the selected element(s). They can be used for decoration (:first-line, :first-letter) or adding elements to the markup (combined with content: ...) without having to modify the markup (:before, :after).

## What are the different modules used in the current version of CSS?

#### Below are

- Selectors
- Box Model
- Backgrounds and Borders
- Text effects
- 2D/3D Transitions
- Animations
- Multiple Column Layout
- User Interface

## What are the different media types allowed by CSS?

- all - for all media type devices
- print - for printers
- speech - for screenreaders that reads page out loud
- screen - for computer screens, tablets, smart-phones, etc

  ```
  @media print {
      h1 {
          background-color: yellow;
      }
  }
  ```

## What is the overflow property in CSS used for?

#### The overflow property specifies what should happen if content overflows an element’s box. This property specifies whether to clip content or to add scrollbars when an element’s content is too big to fit in a specified area.

## What is responsive web design?

#### Responsive design is an approach to web page creation that makes use of flexible layouts, flexible images and cascading style sheet media queries. The goal of responsive design is to build web pages that detect the visitor’s screen size and orientation and change the layout accordingly.

## Explain the concept of specificity in CSS.

#### Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied. Specificity is based on the matching rules which are composed of different sorts of CSS selectors.

## What are contextual selectors?

#### Contextual selectors in CSS allow you to specify different styles for different parts of your document. You can assign styles directly to specific HTML tags, or, you could create independent classes and assign them to tags in the HTML. Either approach lets you mix and match styles.

## What is CSS4?

#### While referring to all new CSS as CSS3 worked for a short time, it doesn’t reflect the reality of where CSS is today. If you read something about CSS3 Selectors, then what is actually being described is something that is part of the [CSS Selectors Level 3](https://www.w3.org/TR/selectors-3/) specification. In fact CSS Selectors is one of the specifications that is marked as completed and a Recommendation. The CSS Working Group is now working on Selectors Level 4 with new proposed features plus the selectors that were part of Level 3 (and CSS 1 and 2). It’s not CSS4, but Level 4 of a single specification. One small part of CSS.-

## CSS-wide values?

#### In addition to the pre-defined keywords that are part of the specification for a property, all CSS properties accept the CSS-wide property values `initial, inherit, and unset`, which explicitly specify defaulting behaviors.

- The initial keyword represents the value specified as the property’s initial value. The inherit keyword represents the computed value of the property on the element’s parent, provided it is inherited.

- The unset keyword acts as either inherit or initial, depending on whether the property is inherited or not.

- A fourth value of revert was added in the Cascade Level 4 specification, but it does not currently have good browser support.

## Flex vs Grid

#### Flex is one direction layout while Grid is two dimension layout

## Credits:

1. https://developer.mozilla.org/en-US/docs/Web/CSS
2. https://www.javatpoint.com/css-interview-questions
3. https://www.edureka.co/blog/interview-questions/css-interview-questions/#three
4. https://css-tricks.com/css4/
5. https://rachelandrew.co.uk/archives/2016/09/13/why-there-is-no-css4-explaining-css-levels/
6. https://drafts.csswg.org/selectors-4/
