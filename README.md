**JLexer Documentation**

### Welcome to JLexer!

**Installation:**

*Web:*
- **CDN:**
  ```html
  <script src="CDN"></script>
  ```
- **Local:**
	- *DOWNLOAD LINK HERE*
	- `<script src="CDN"></script>`

**Getting Started:**

JLexer simplifies the process of splitting input into tokens.

**Defining Tokens:**
```javascript
const JLexer = require("jlexer");

const config = {
	do_paren_leveling: true,
	do_brace_leveling: true,
	do_bracket_leveling: true,
};

const tokens = {
	STRING: /\"[^\"]*\"/,
	// Add more as needed.
};

const tokenized_output = JLexer(tokens, config);
```

**Configuration:**
- Customize leveling for brackets, braces, and parentheses in the configuration.

**Token Definitions:**
- Define token regexes based on your specific needs.

JLexer v0.0.1 by Defying Gravity
