What are Pseudo-elements?

```
They start with :: and are used to style a specific part of an element.

Unlike pseudo-classes (which style a state like hover), pseudo-elements style a part of the content itself.
```

✨ Common Pseudo-elements
```
📝 1. ::before
```
Adds content before an element.

✅ Example
```
p::before {
  content: "👉 ";
  color: blue;
}
```
👉 Adds a symbol before every paragraph

📝 2. ::after

Adds content after an element.

✅ Example
```
p::after {
  content: " ✔";
  color: green;
}
```
👉 Adds a checkmark after every paragraph

📝 3. ::first-letter

Styles only the first letter of text.

✅ Example
```
p::first-letter {
  font-size: 30px;
  color: red;
}
```
👉 First letter becomes bigger and red

📝 4. ::first-line

Styles only the first line of text.

✅ Example
```
p::first-line {
  font-weight: bold;
  color: purple;
}
```
👉 First line becomes bold and purple

📝 5. ::selection

Styles the text selected by the user.

✅ Example
```
::selection {
  background: yellow;
  color: black;
}
```
👉 Highlighted text changes color

🔥 Combined Example
```
h1::before {
  content: "🌟 ";
}

h1::after {
  content: " 🌟";
}

p::first-letter {
  font-size: 35px;
  color: red;
}

::selection {
  background: lightblue;
}
```
👉 Heading gets stars, paragraph first letter becomes large, selected text changes color

⚡ Difference Between Pseudo-class and Pseudo-element

| Pseudo-class     |	Pseudo-element    |
------------------ |----------------------|
|Starts with :    |	Starts with ::        |         
|Styles a state   | 	Styles a specific part|
|Example: :hover	 |   Example: ::before    |