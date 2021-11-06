## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/singleproject/video/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/singleproject/video/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
<!DOCTYPE html>
<html>

<head>
	<title>Getting Clients IP</title>
	<style>
		p, h1 {
			color: green;
		}
	</style>
	<script src=
"https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js">
	</script>

	<script>
		/* Add "https://api.ipify.org?format=json" statement
		this will communicate with the ipify servers in
		order to retrieve the IP address $.getJSON will
		load JSON-encoded data from the server using a
		GET HTTP request */

		$.getJSON("https://api.ipify.org?format=json",
										function(data) {

			// Setting text of element P with id gfg
			$("#gfg").html(data.ip);
		})
	</script>
</head>

<body>
	<center>
		<h1>GeeksforGeeks</h1>
		<h3>Public IP Address of user is:</h3>

		<p id="gfg"></p>

	</center>
</body>

</html>
