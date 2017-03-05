[![Build Status](https://travis-ci.org/stilesb/github-pages-https-example.svg?branch=master)](https://travis-ci.org/stilesb/github-pages-https-example)

# github-pages-https-example

*For demonstrating how to setup an HTTPS-enabled GitHub Pages website*

## Setup

- Create a GitHub user account on `https://www.github.com`
- Create a repository
- Clone the repository locally

`git clone https://github.com/stilesb/github-pages-https-examples.git`

- Add a `docs` folder and include an `index.html` file there

```bash
$ mkdir docs
$ cat <<EOF>> docs/index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>GitHub Pages HTTPS Example</title>
    <!--[if IE]>
        <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
</head>
<body>
    <h1>GitHub Pages HTTPS Example</h1>
</body>
</html>
EOF
```

- Navigate to the GitHub repository settings and head to "Options" > "GitHub Pages" and select the `master branch /docs folder` source
- Optionally add your custom domain - if you do so, you'll need to use CloudFlare for SSL, see below for more instructions
- Optionally choose a theme in "Options" > "GitHub Pages"
- Click "Save"
- Add new two records to your domain DNS. In this example I'm using Google Domains.
- Browse to your site's URL - it should be working. But if you have a custom domain you'll have SSL errors.

### Custom Domains

If you're using a custom domain and/or would like SSL support, here, we're going to set this up using CloudFlare.

- Head over to `https://www.cloudflare.com` and register a new account
- Create a site, entering the custom domain of your site
- Transfer your DNS entries from your current DNS provider to CloudFlare. There should be one "Type A" entry (name is your custom domain, value is the GitHub IP address). The second will be a "CNAME" entry (name is "www" and value is your GitHub Pages account URL)
- When done, add pages rules to enforce HTTPS and forward your base URL to www.
- You're done!
