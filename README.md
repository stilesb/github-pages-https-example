# github-pages-https-example

**For demonstrating how to setup a HTTPS-enabled GitHub Pages website**

## Setup

- Create a GitHub repository on https://www.github.com (or locally on the terminal with `git`)
- Clone the repository e.g. `git clone https://github.com/civiclabsconsulting/github-pages-https-examples.git`
- Add a `docs` folder and include an `index.html` file there

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <title>HTML5 Boilerplate</title>
    <!--[if IE]>
        <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
</head>

<body>
    <h1>HTML5 Boilerplate</h1>
    <!-- Begin Cookie Consent plugin by Silktide - http://silktide.com/cookieconsent -->
    <script type="text/javascript">
        window.cookieconsent_options = {
            "message": "This website uses cookies to ensure you get the best experience on our website",
            "dismiss": "Got it!",
            "learnMore": "More info",
            "link": null,
            "theme": "light-bottom"
        };
    </script>

    <script type="text/javascript" src="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/cookieconsent.min.js"></script>
    <!-- End Cookie Consent plugin -->

</body>

</html>
EOT
```

- Navigate to the GitHub repository settings and navigate to "Options" > "GitHub Pages" and select the `master branch /docs folder` source
- Optionally choose a theme in "Options" > "GitHub Pages"
- Click "Save" and you're done!
