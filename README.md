#### HTML elements used by flashcards.js:
i (section header, preceeds section content)

p (section content, contains answers)

b (answer)

#### Customization
In `flashcards.js`, the following defaults can be changed:

```javascript
{
  answerButtonClasses: "p, b",
  openallButtonClasses: "p, .openall",
  baseClass: ".flashcards",
}
```

Some struture needs to be followed in the HTML:
  - `baseClass` needs to wrap everything
  - Section content is the first (`<p>`) sibling of the section header (`<i>`)
  - An answer is not linked to a question other than being next to it on the page.
  - Some new lines are automatically added after answers.




