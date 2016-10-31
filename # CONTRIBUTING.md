# CONTRIBUTING.md

Contributors are generally employees of Sumo Logic. Community Members may make suggestions that contributors may choose the support.

There are two types of contribution. The first is to contribute new content. The second is by enhancing the site.

## Updating Content
Jekyll is a static site generator that includes the Liquid template engine to create data-driven sites. So using Liquid’s template language I was able to populate open-source projects into the site using data read from a Yaml file. This feature allows our internal teams to quickly update the site without having to muck in the code. 

Note: You do not need to install Jekyll to update these .yml files. 

Updating content is a simple matter of editing one of two .yml files. 

experts.yml - updates the sumo-experts.html page
partners.yml - updates the partners.html page

A typical entry looks like:


 - title: "Sumo Report Generator"
   repo_description: "Tool that allows a user to execute multiple searches, and compile the data into a single report."
   url: "https://github.com/SumoLogic/sumo-report-generator"

The only catch is that the dash character ( - ) must be indented by one space or the build will fail. Otherwise, just replace the title, description and text with your new text.
 
## Updating the Site

There are some obvious enhancements I haven't gotten around to yet. If you're so inclined, you'll first need to install the Jekyll Gem on your local machine. This, of course assumes you have Ruby already configured. See the Jekyll documentation for details.

### Directory Layout 

Most html files are stored in the root directory. Jekyll generates _site, _layouts and other directories. You generally will not touch these as they are generated on the fly. Here's a description of directories you might edit:

* _data - contains the .yml files used to populate the site
* _includes - contains the HTML Head, the site header markup, the footer and other includes.
* images - site images.
* css - site css including Bootstrap.css
* js - Supporting Bootstarp Javascript files.


## How to contribute?

1. Before starting work on a new feature, enhancement, or fix, please create an issue and optionally assign it to yourself or a developer.
2. Fork the repository and make your changes against the 'development' branch (not master).
3. After making your changes in your fork, run tests and ensure that the page looks good and works with all supported browsers.
4. If you have made a series of commits into the 'development' branch, please try to squash them into a small number of commits.
5. Issue a Pull Request against the 'development' branch (not master).

The admins will review your code and may optionally request conformance, functional or other changes. Work with them to resolve any issues.
Upon acceptance, your code will be merged into the master branch and will become available for all.