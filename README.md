# github-pages-https-example

**For demonstrating how to setup a HTTPS-enabled GitHub Pages website**

## Setup

1. Create a GitHub repository on https://www.github.com (or locally on the terminal with `git`)
2. Clone the repository e.g. `git clone https://github.com/civiclabsconsulting/github-pages-https-examples.git`
3. Add a `docs` folder and include an `index.html` file there

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

5. Navigate to the GitHub repository settings and navigate to "Options" > "GitHub Pages" and select the `master branch /docs folder` source
6. Click "Save" and you're done!
