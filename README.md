Cloudscaling - Blog
========

This project uses [Ruby](https://www.ruby-lang.org/en/downloads/) , [Sass](http://sass-lang.com) and [Ruby-oembed](https://github.com/judofyr/ruby-oembed) to preprocess and convert oembed to iframe. [s3_website](https://github.com/laurilehmijoki/s3_website) is mainly used to create redirects and push files to staging and production. [Bundler] is a package manager that makes versioning Ruby software like Jekyll a lot easier and manage dependencies.

Getting Started
---------------

1. Clone this repo locally.
2. Jekyll requires the Ruby language. If you have a Mac, you've most likely already got Ruby. If you open up the Terminal application, and run the command ruby --version you can confirm this. Your Ruby version should be at least 2.0.0. If you've got that, you're all set. Otherwise, follow [these instructions to install Ruby](https://www.ruby-lang.org/en/downloads/).
3. `cd` to the project root
4. Run `gem install bundler` to install the bundler
5. Run `bundle install` to install the build dependencies.
6. Now, run `bundle exec jekyll serve build --watch` to start jekyll and watch for file changes.
7. Open a browser `http://127.0.0.1:4000/`


Blog Deployment Notes
====================
The following commands will run as a dry-run, enter 'y' to deploy
1. Run `sh _deploy/deploy.sh stage` to push to staging
2. Run `sh _deploy/deploy.sh production` to push to production

Blog Configuration Notes
====================
[s3_website](https://github.com/laurilehmijoki/s3_website) needs both Ruby and Java to run. (S3_website is partly written in Scala, hence the need for Java.) The site uses s3_website to deploy files.
The configuration files are stored in `_s3_prod_config` and `_s3_stage_config`. 
In order to change the S3 bucket, update `s3_website.yml` 

Jekyll Theme Notes
====================

1. All project assets (pdf, sheets and images) reside within the jekyll assets folder `assets`
2. Plugins are under `_plugins`
3. The `_includes` folder has the different partials for the site such as:
    - head
    - header.html
    - pagination.html
    - search.html
4. The `_layouts` folder has the different layouts for the site such as:
    - a regular page - page.html
    - a single post - post.html
    - authors page - single_author.html
5. The `blog` folder has all the posts, the sub folders are use to replicate the categories from the main blog. Example: 
    - cloud-computing/_posts/2015-08-11-cloud-youre-doing-it-wrong.markdown => HOST/blog/cloud-computing/cloud-youre-doing-it-wrong/