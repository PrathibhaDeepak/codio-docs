---
title: "Markdown content editing "


---

## Cheat Sheet
Please refer to the **Callout** section of the Cheat Sheet. If you have not done so already, fork [this starter pack](https://codio.com/home/starter-packs/cb114a27-d88e-4b74-a2a0-518ccb30dc44/) into your own account. You should select the **Use Pack** option to create the project.

Content can be written in

- **Markdown** - the recommended option and described on this page
- **HTML** allowing more detailed control but requiring more time; described on the next page.

When you are in edit mode, you can select a section by

- using the navigation buttons in the header area
- selecting a section from the section list

<img alt="editnav" src="/img/guides/editnav.png" class="simple"/>


## Renaming the Section
You can rename your section by clicking on the section title in the header area.

## Writing content
You can then start writing your content in the main content area.

## Markdown
For those of you not familiar with Markdown, it is an extremely easy way of writing content without having to worry about HTML.

When in play Mode, your content is rendered as students will see it. You can also override the default CSS styling. Go to Tools>Guide>Add Custom CSS
<img alt="Guide CSS" src="/img/guides/guidecss.png" class="simple"/>

'Reset Custom CSS' will restore the default CSS styling

Click here for details on how to insert [images, videos and hyperlinks](/content/authoring/page-edit/imvid).

Here is a summary of the Markdown formatting codes

## Headers/Titles
To display a header or title, you can use the `#` character at the start of the line. The more `#` characters you add, the smaller the font.

```markdown
# Big title
## Smaller title
### Even smaller title
#### etc.
```

## Bold and Italic
To create bold or italic text, you use `**` and `*` either side of the respective words.

```markdown
I want to say that **this is really important**, you know
I *really* like chocolate
```

## Bullet Lists
To create a list of bullet points, you start the line with a `-`

```markdown
- Bullet 1
- Bullet 2
- Bullet 3
- etc
```

## Numbered Lists
To create a numbered list, you start the line with a `1.` The numbers are automatically calculated for you.

```markdown
1. Item 1
1. Item 2
1. Item 3
1. etc
```

## Code Blocks
If you want to show some code, styled with the courier font, in a box and with syntax highlighting applied you surround your code block with three backticks `` ``` ``. For example, the following javascript snippet

```js
var i;
for(i = 0; i < 10; i++) {
   document.write(i);
}
```

is written as

`` ```js``
var i;
for(i = 0; i < 10; i++) {
   document.write(i);
}
`` ``` ``

Note that you can specify a language type after the top 3 back ticks. Entering `python ` after the backticks would apply syntax highlighting for python. Many languages are supported. [See a full list of supported languages here](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml). You should search for your language and then use the `alias` shown.

## Code Segments
If you want to insert a piece of code inline with the rest of your text, then you use a single \` (backtick) character either side of the text. For example,

We can define a variable `var x;` if we like

... is written in markdown as

We can define a variable \`var x;\` if we like


## Indented Lists
If you want to indent a list, then indent just 2 spaces and it will indent.

```markdown
  - Bullet 1
  - Bullet 2
  - Bullet 3
  - etc
```

## Callout Blocks
If you want to show a callout block a number of options are available and others can be easily added if required

  - important
  - info
  - warning
  - topic
  - definition
  - challenge
  - guidance
  - meetup
  - hackathon
  - create
  - calendar
  - growthhack
  - xdiscipline
  - debugging

e.g.

```
|||info
# My Title

Some text

|||
```

<img alt="calloutinfo" src="/img/guides/callout_info.png" class="simple"/>

The **Guidance** callout block is only visible in play mode to designated teachers within a class. It is not visible for students.


## Hyperlinks, Images, Videos & iframes
We describe these in [this section](/content/authoring/page-edit/imvid).

## HTML
You can include HTML tags

## Latex / MathJax

Latex is supported using [MathJax](http://www.mathjax.org/). For example

```markdown
When $a \ne 0$ there are two solutions to $(ax^2 + bx + c = 0)$ and they are $x = {-b \pm \sqrt{b^2-4ac} \over 2a}$

and for multiple lines we do the following

$$
y=x^2
y=\frac{x^2}{x+1}
$$
```

[Click here](/content/authoring/page-edit/latex) for more details on Latex and Mathjax.

<img alt="MathJax" src="/img/guides/mathjax.png" class="simple"/>

Inline math equations are encapsulated in a single `$` like this: $\omega = d\phi / dt$.


## Cheat Sheet

Check out our [Cheat Sheet](https://codio.com/home/starter-packs/cb114a27-d88e-4b74-a2a0-518ccb30dc44/) and **Use Pack** to create the Cheet Sheet project in your Codio account.