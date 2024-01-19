# JLexer Documentation

## Welcome to JLexer!

### Installation:

#### Web:
```html
<script src="https://cdn.jsdelivr.net/gh/xDefyingGravity/JLexer@main/jlexer.min.js"></script>
```
Local:

	• <script src="jlexer.min.js"></script>
Getting Started:

JLexer simplifies the process of splitting input into tokens.

## Defining Tokens:
```javascript
const JLexer = require("jlexer");

const config = {
  do_paren_leveling: true,
  do_brace_leveling: true,
  do_bracket_leveling: true,
};

const tokens = {
  STRING: /\"[^\"]*\"/,
  // Customize the following tokens as needed.
  // ...
};

const tokenized_output = JLexer(tokens, config);
```
## Configuration:

The configuration object (config) allows you to control bracket, brace, and parenthesis level tracking. Set to true to enable or false to disable.
```javascript
const config = {
   do_paren_leveling: true,
   do_brace_leveling: true,
   do_bracket_leveling: true,
}
```
## Token Definitions:

Define token regexes based on your specific needs, for example:
```javascript
const tokens = {
    NUMBER: /\d+/,
    PLUS: /\+/
}
```
## How to run and tokenize the input:
```javascript
const codeExample = '2+3';
const tokenizedOutput = JLexer(tokens, config);
console.log(tokenizedOutput);
```
Version:

	•	JLexer v0.0.1 by Defying Gravity
