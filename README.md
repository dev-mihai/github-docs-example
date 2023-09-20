# Crafting Stellar Documentation

## 1. Embrace the Power of Codeblocks

Using codeblocks in markdown is not just helpful; it's a game-changer. It facilitates seamless **copying, pasting, and sharing** of code snippets. An adept Cloud Engineer knows the importance of incorporating Codeblocks regularly. 

Why? Because it:
- Makes it straightforward for peers to replicate or delve into issues.
- Enhances readability and comprehension.

Here's how you create a codeblock in markdown using three backticks(```):

```
import json
import requests
import urllib3

urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)

# Global Static Variables
HOST = morpheus["morpheus"]["applianceHost"]
INTERNAL_HOST = morpheus["customOptions"]["internalHost"]
TOKEN = morpheus["morpheus"]["apiAccessToken"]
...
```

And when you can, enhance your code with syntax highlighting:

```python
import json
import requests
import urllib3

urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)

# Global Static Variables
...
```

## 2. Incorporate Engaging Visuals

Add images to make your documentation more engaging. To do this:
- Use `!` followed by alt text in `[]` (a short description of the image).
- Then, wrap the image link in `()`.

### Example:
![Octocat smiling and raising a tentacle](https://myoctocat.com/assets/images/base-octocat.svg)

If resizing is needed, adopt the following method:

<img width="200px" src="https://myoctocat.com/assets/images/base-octocat.svg" />

Remember, for an articulate documentation, use codeblocks not just for code but also for console errors:

```bash
Traceback (most recent call last):
...
RuntimeError: This is a custom error message
```

> An exemplar representation of an error using a bash codeblock.

## 3. Harness GitHub's Task Lists

GitHub has enriched Markdown to include interactive task lists. Check them off as you progress!

- [x] Achieved Step 1
- [ ] In Progress: Step 2
- [x] Accomplished Step 3

## 4. Enliven with Emojis (Optional yet Fun!)

GitHub Flavored Markdown (GFM) introduces emoji shortcodes. A sprinkle of emojis can lighten up the documentation:

| Description           | Shortcode                   | Emoji   |
| --------------------- | --------------------------- | ------- |
| Cloud                 | `:cloud:`                   | ☁️      |
| Cloud with lightning  | `:cloud_with_lightning:`    | 🌩️     |

## 5. Tables: Simplifying Data Representation

To craft tables:

```md
| Description           | Shortcode                   | Emoji   |
| --------------------- | --------------------------- | ------- |
| Cloud                 | `:cloud:`                   | ☁️      |
| Cloud with lightning  | `:cloud_with_lightning:`    | 🌩️     |
```

Remember:
- The `|` key is typically above the Return or Enter key.
- However, it might differ depending on your keyboard layout.

![RedHat Logo](/assets/redhat-icon.svg)

![Morpheus Logo](/assets/morpheus-logo-v2.svg)

## Essential References

- [GitHub's Official Flavored Markdown Guide](https://github.github.com/gfm/).
- [A Comprehensive Writing and Formatting Syntax by GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting=syntax#quoting-text).
- [GitHub's Task List Guide](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists).<sup>[1]</sup>
