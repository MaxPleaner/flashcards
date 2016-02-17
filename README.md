#### Setup

Depends on jQuery and the `flashcards.js` script.

Require these in HTML page and then initialize with:

```html
    $(function(){Flashcards.begin()})
```

#### Example

Clone the repo and open `flashcards.html` to see an example.

Note that this includes some styles.

#### HTML elements used by flashcards.js:
`<i>` (section header, preceeds section content)

`<p>` (section content, contains answers)

`<b>` (answer)

#### Customization

In `flashcards.js`, the following defaults can be changed:

```javascript
{
  answerButtonClasses: "p, b",
  openallButtonClasses: "p, .openall",
  baseClass: ".flashcards",
}
```

#### Understanding the options

For `answerButtonClasses` and `openallButtonClasses`, buttons are
automatically created and put before the specified element on the page.

`answerButtonClasses` elements (`<p>` and `<b>`) will have "toggle" buttons
automatically added before them.

`openallButtonClasses` elements (`<p>`, `.openall`) have an `open all` button
added. This button will toggle all of the answers or sections which the
`openallButtonClasses` element contains.

Some examples from `flashcards.html` to explain `openallButtonClasses`:
  - The `.openall` contains many `<p>` sections, and therefore
there will be a button to toggle all of the `<p>` sections at once.
  - For each `<p>`, a button is added to toggle all the `<b>` elements which
  it contains


#### Additional HTML structure to follow
Some struture needs to be followed in the HTML:
  - `baseClass` needs to wrap everything
  - Section content is the first (`<p>`) sibling of the section header (`<i>`)
  - An answer is not linked to a question other than being next to it on the page.
  - Some new lines are automatically added after answers.





