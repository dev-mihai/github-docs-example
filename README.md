# Writing Good Documentation

## Step 1 - Using Codeblocks.

Codeblocks in markdown make it *very easy* for tech people to **copy, paste, and share** code.
A Good __Cloud Engineer__ uses Codeblocks whenever possible.

Because it allows others to copy and paste their code to replicate or research issues

In order to create code blocks in markdown you need to use three backticks(`)
```
import json
import requests
import urllib3

urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)

## Global Static Variables
HOST = morpheus["morpheus"]["applianceHost"]
INTERNAL_HOST = morpheus["customOptions"]["internalHost"]
TOKEN = morpheus["morpheus"]["apiAccessToken"]
AWS_KEY = morpheus["customOptions"]["awsKey"]
AWS_SECRET = morpheus["customOptions"]["awsSecret"]
AWS_VPC = morpheus["customOptions"]["awsVpc"]
AWS_REGION = morpheus["customOptions"]["awsRegion"]
INTERNAL_URL = "https://%s" % (INTERNAL_HOST)
```

- When you can, you should attempt to apply syntax highlighting to your codeblock
```python
import json
import requests
import urllib3

urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)

## Global Static Variables
HOST = morpheus["morpheus"]["applianceHost"]
INTERNAL_HOST = morpheus["customOptions"]["internalHost"]
TOKEN = morpheus["morpheus"]["apiAccessToken"]
AWS_KEY = morpheus["customOptions"]["awsKey"]
AWS_SECRET = morpheus["customOptions"]["awsSecret"]
AWS_VPC = morpheus["customOptions"]["awsVpc"]
AWS_REGION = morpheus["customOptions"]["awsRegion"]
INTERNAL_URL = "https://%s" % (INTERNAL_HOST)
```

## Adding Images
You can display an image by adding ! and wrapping the alt text in [ ]. Alt text is a short text equivalent of the information in the image. Then, wrap the link for the image in parentheses ().
### Example:
![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)

If you need to resize an image, use the following:

<img width="200px" src="https://myoctocat.com/assets/images/base-octocat.svg" />

Good cloud Engineers use codeblocks for both Code and Errors that appear in the console.

```bash
Traceback (most recent call last):
2: from /usr/bin/irb:23:in '<main>'
1: from (irb):1
RuntimeError: This is a custom error message
```

> Here is an example of using a codeblock for an error that appears in bash.

## Step 3 - Use Github Flavoured Task Lists

Github extends Markdown to have a list where you can check off items. <sup>[1]</sup>
- [x] Finish Step 1
- [ ] Finish Step 2
- [x] Finish Step 3

## Step 4 - Use Emojis (Optional)

GitHub Flavored Markdown (GFM) supports emoji shortcodes.

Here are some examples:
| Name | Shortcode | Emoji |
| --- | --- | --- |
| Cloud | `:cloud:` | :cloud: |
| Cloud with lighting | `:cloud_with_lightning:` | 🌩️ |

## Step 5 - How to create a table

```md
| Name | Shortcode | Emoji |
| --- | --- | --- |
| Cloud | `:cloud:` | :cloud: |
| Cloud with lighting | `:cloud_with_lightning:` | 🌩️ |
```
Github extends the functionality of Markdown tables to provide more alignment and table cell formatting options. [<sup>[2]</sup>](#external-references)

- Make note of where the pipe keyboard key is located.
- It should appear above return or enter key
- but it may vary based on your keyboard layout.

![Photo of the pipe character on our keyboard](assets/pipe-char.jpg)

[Secret Window Hidden Garden](secret-window/hidden-garden.md)

## References
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/).
- [Basic writing and formatting syntax (Github Flavored Markdown)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting=syntax#quoting-text).
- [GFM - Tasks Lists](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists).<sup>[1]</sup>
