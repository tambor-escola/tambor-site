# Enterprise Intelligence Platform Site

Welcome to the repository for the Enterprise Intelligence Platform (EIP) website by BAO Systems.

## Technology

* The web site is built with [Jekyll](https://jekyllrb.com/).
* It uses the [Minima](https://github.com/jekyll/minima) theme. The site was initated as a fork of the Minima theme code.
* Jekyll requires [Ruby](https://www.ruby-lang.org/).
* Ruby dependencies are managed with the [bundler](https://bundler.io/) tool.
* Jekyll uses the [Liquid](https://shopify.github.io/liquid/) template language.

## Install Jekyll and bundler

The site generator requires Jekyll and the bundler dependency management tool.

Set environment variables in `.bashrc`.

```
export GEM_HOME="$HOME/.gem"
export PATH="$GEM_HOME/bin:$PATH"
```

Install Jekyll and bundler.

```sh
gem install jekyll bundler
```

## Get started

From the root directory of the repository checkout, install gems.

```sh
bundle install
```

Build the site.

```sh
bundle exec jekyll build
```

Serve the site.

```sh
bundle exec jekyll serve
```

Open the web site in a browser at the default location.

```
http://127.0.0.1:4000
```

## Deployment

* The site is automatically built and deployed with Bitbucket Pipelines.
* On every commit to the source code repository, the pipeline is trigged and changes will be reflected online after about a minute.
* The static web site hosted from an AWS S3 bucket `bao-ap-web-site`.
* The S3 website URL is http://bao-ap-web-site.s3-website-eu-west-1.amazonaws.com.
* The public URL is https://ap.baosystems.com.

## Structure

The structure of the repository is described in the following section.

## Images

* Format: PNG
* Location: `/assets/images`
* Naming: Lowercase, hyphen-separated
* Avoid scrollbars if possible.
* Small image size width is 550 px.
* Large image size width is 1200 px.

### Single column

* Width: 1200px

### Two column

* Width: 550px
* Width/height ratio: 1.4

### Connector icon

* Height: 64px

## Screencasts

* Screencasts are created with [Screencastify](https://www.screencastify.com/) and the Screencastify Chrome extension.
* Record a tab.
* Set resolution to 1280 x 720 (720p).
* Set max frame rate to 60.
* Disable show drawing tools.
* Videos are hosted on AWS S3 in the `bao-ap-web-site` bucket under media > video.

Test README update
