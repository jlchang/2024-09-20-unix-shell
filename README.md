# 2024-05-09 The Unix Shell (pilot) session website github repo

View the [session website][session-website].

This repository is based on The Carpentries' ([Software Carpentry][swc-site], [Data Carpentry][dc-site], and
[Library Carpentry][lc-site]'s) [template][template-link] for creating websites for workshops. This IS NOT the [session CONTENT][session-link] [github][session-github-link].

1. **Please _do not fork this repository directly on GitHub._** Instead, please use GitHub's
   "template" function following [the instructions for][creating-a-repository] to copy the
   `workshop-template` [repository][template-link] and customize it for your workshop.

2. Please *do your work in your repository's `gh-pages` branch*, since that is what is
   [automatically published as a website by GitHub][github-project-pages].

The pages on [customizing your website][customization],
the [FAQ][faq],
and the [design notes][design] have more detail on how this template works and why.
And please note:
if teaching Git,
please [create a separate repository][setting-up-a-separate-repository-for-learners]
for learners to practice in.

## Video Tutorial

There is a [YouTube video](https://www.youtube.com/watch?v=_Ag1JiZzyUQ) that demonstrates how to
create a workshop website.


### Working locally

> Note: you don't have to do this, if you have already updated your site using the web interface.
> Working locally may be more efficient if you are making interdependent changes in multiple files so that
> each file update does not trigger a separate website build job. (or, when using the web interface,
> create a branch before making interdependent changes then merge to `gh-pages`)


If you are already familiar with Git, clone the repository to your desktop:

```shell
git clone https://github.com/your_username/YYYY-MM-DD-site
```

Then edit `index.md`,`_config.yml`, and `schedule.html` following the [customization instructions][customization], 
and push your changes back to the repository.

In order to view your changes once you are done editing, if you have bundler installed (see the
[installation instructions][installing-software]), you can preview your site locally with:

```shell
make serve
```
and go to <http://0.0.0.0:4000> to preview your site.

Before pushing your changes to your repository, we recommend that you also check for any potential
issues with your site by running:

```shell
make workshop-check
```

Once you are satisfied with the edits to your site, commit and push the changes to your repository.
A few minutes later, you can go to the GitHub Pages URL for your workshop site and preview it. An example URL might look like `https://gvwilson.github.io/2016-12-01-oomza`. 
[The finished page should look something like this](fig/completed-page.png?raw=true).

<!--links set up for this session-->
[session-link]: https://jlchang.github.io/2024-05-09-Unix_Shell_pilot/
[session-github-link]: https://github.com/jlchang/2024-05-09-Unix_Shell_pilot
[session-website]: https://broadinstitute.github.io/2024-05-09-Unix_Shell/

<!--persistent links-->
[template-link]: https://github.com/carpentries/workshop-template
[creating-a-repository]: https://github.com/carpentries/workshop-template?tab=readme-ov-file#creating-a-repository
[customization]: https://carpentries.github.io/workshop-template/customization/index.html
[swc-site]: https://software-carpentry.org
[dc-site]: https://datacarpentry.org
[lc-site]: https://librarycarpentry.org
[design]: https://carpentries.github.io/workshop-template/design/index.html
[faq]: https://carpentries.github.io/workshop-template/faq/index.html
[github-project-pages]: https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site
[setting-up-a-separate-repository-for-learners]: https://github.com/carpentries/workshop-template?tab=readme-ov-file#setting-up-a-separate-repository-for-learners
[installing-software]: https://github.com/carpentries/workshop-template?tab=readme-ov-file#installing-software
[lesson-example]: https://carpentries.github.io/lesson-example/
