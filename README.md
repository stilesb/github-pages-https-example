# github-pages-https-example

**For demonstrating how to setup a HTTPS-enabled GitHub Pages website**

## Setup

- Create a GitHub repository on https://www.github.com (or locally on the terminal with `git`)
- Clone the repository e.g. `git clone https://github.com/civiclabsconsulting/github-pages-https-examples.git`
- Add a `docs` folder and include an `index.html` file there

```
mdkir docs
cat <<EOT>> docs/index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>HTML5 Boilerplate</title>
    <link rel="stylesheet" href="css/style.css">
    <!--[if IE]>
        <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
</head>
<body>
     <h1>HTML5 Boilerplate</h1>
</body>
</html>
EOT
```

- Navigate to the GitHub repository settings and navigate to "Options" > "GitHub Pages" and select the `master branch /docs folder` source
- Optionally choose a theme in "Options" > "GitHub Pages"
- Click "Save" and you're done!
