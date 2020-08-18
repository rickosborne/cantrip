# Cantrip

Cantrip helps tabletop RPG authors iterate on their work: **C**ontent **A**utomatio**N** for **T**abletop **R**oleplaying **I**teration **P**rocesses.

## Will Cantrip help me?

Cantrip is targeted at authors with at least moderate familiarity with source code and build tools.
You don't necessarily need to be a programmer, but you will need to know how to get console/terminal apps installed and configured, and you'll need to have at least introductory Git skills.

If you've got those skills, and you have an idea for a tabletop RPG module, Cantrip may be of help.

## What skills do I need?

At the most basic, just to create a project:

* Proficiency with Markdown
* Familiarity with Git
* Familiarity with YAML or JSON, or at least a passing understanding of structured data

If you want to be able to develop your work and see changes locally as you make them:

* Familiarity with the console/terminal and how to install console apps

If you want to really dig into making the published modules look like your own personal branding:

* Proficiency with CSS (or better: SASS)
* Proficiency with HTML

If you want to add more automation, so you can do more interesting things:

* Proficiency with Typescript (or at least Javascript)

## What are some alternatives?

To the best of my knowledge at this time (2020-Aug), there aren't any other out-of-the-box solutions for going from human-readable tabletop RPG text to publishable PDF.
Most RPG-related resources will be template files, such as MS Word or Adobe InDesign.

More robust publishing systems aren't really aimed at gaming at all.
With some work, however, they could probably offer more features than Cantrip, as Cantrip keeps a narrow focus.
Here are a few options:

* [Electric Book](https://github.com/electricbookworks/electric-book)

  This was one of the inspirations for Cantrip, and we share a number of common tools.

* [Gitbook](https://www.gitbook.com/)

  This has become a hosted solution, which was a deal-breaker for me.

* [Hugo](https://gohugo.io/documentation/)

  Similar to Jekyll, which underpins Cantrip and Electric Book, Hugo is mostly just a static site generator.
  It would be fine for local development, but I wanted a solution more compatible with the magic of GitHub Pages.
  (Though I admit, as Cantrip gains more templating functionality, and more of the rendered content is checked in, the distinction is not as meaningful.)

## Getting Started

1. Install `node` and `npm`:
  * [Installers here, if you're not sure.](https://nodejs.org/en/download/)
  * [Technical instructions here, if you're comfortable.](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
2. Install Dart Sass:
  * [Dart Sass explanation](https://sass-lang.com/dart-sass)
  * [Sass installation instructions](https://sass-lang.com/install) — Careful!  Even though you're working with NodeJS, you _don't_ want the Node/npm version of Sass.  It's too slow!  You want Dart Sass, trust me.
3. Fork the [Cantrip repository](https://github.com/rickosborne/cantrip/).
  * If you already have an existing repo and don't want to fork Cantrip, you'll need to copy over all the files to your repo.
    You'll likely need to do some integrating with `package.json` and `_config.yml` if you already have them.
    The rest should be pretty straightforward.
4. Update the following files:
  * `package.json` — Add your name, your project's name, and update the URLs.
  * `_config.yml` — Update the repository and site information at the top of the file.
5. Commit and push your changes to your own GitHub repo (fork).
6. [Configure your GitHub repo to automatically publish changes with GitHub Pages.](https://docs.github.com/en/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#choosing-a-publishing-source)

If you want to work locally, there's really only one additional step:

7. From a console/terminal in your local directory, run the following:

       npm start

   This will start up a local web server, which you can visit at:
   
   > [127.0.0.1:4000](http://127.0.0.1:4000/)
                                                                                                                                  

                                                                                                                                  
## Licensing

See the dedicated [License](LICENSE.md) document.
