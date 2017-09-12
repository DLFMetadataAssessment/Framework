# DLF-AIG Metadata Assessment Working Group

**This is the repository contains all content related to the Metadata Assessment Framework developed by the DLF AIG Metadata Working Group and is a subsection of the DLF AIG MWG Website. The work contained in this site was started in 2016 as part of the Environmental Scan and is designed to provide high level guidance for those looking to analyze their existing metadata. This site deploys as a submodule of the [Sandbox](https://github.com/DLFMetadataAssessment/Sandbox) site to [https://dlfaigmwgdev.herokuapp.com/Framework](https://dlfaigmwgdev.herokuapp.com/Framework) for viewing.**

**See the Live/Production/Current site at http://dlfmetadataassessment.github.io/ and the Repository for the live site at https://github.com/DLFMetadataAssessment/DLFMetadataAssessment.github.io/**

## Intro

This site was developed by the [Digital Library Federation Assessment Interest Group Metadata Assessment Working Group](https://groups.google.com/forum/#!forum/dlf-aig-metadata-assessment-working-group), a.k.a. the DLF Metadata Assessment Working Group.

We want the [DLF Metadata Assessment Working Group site](http://dlfmetadataassessment.github.io/) and the information contained therein to be a living document. Working Group members will continue to add resources, recommendations, and information to this website as well as to our working documents. If you want to make a comment, suggestion, correction or update, you can:

  * [submit a pull request to this website](https://github.com/DLFMetadataAssessment/DLFMetadataAssessment.github.io/pulls),

  * [open a GitHub issue on this repository](https://github.com/DLFMetadataAssessment/DLFMetadataAssessment.github.io/issues),

  * [submit updates via Google Form](https://docs.google.com/forms/d/e/1FAIpQLSe1SG3Yv3WYotd8QlC_e1jp6q0KMQ836LLHjBojXwsQJwiZGQ/viewform?embedded=true)

  * [send a message to our Google Group](https://groups.google.com/forum/#!forum/dlf-aig-metadata-assessment-working-group),

  * [join one of our calls](https://wiki.diglib.org/Assessment:Metadata).

Anyone and everyone is welcomed to take part in the DLF AIG Metadata Working Group. Use the link below to find out more about the group or get involved.

  * [our DLF wiki page](https://wiki.diglib.org/Assessment:Metadata)

## Contributing via this GitHub Repository

This is a group effort and we welcome any and all contributions. This information below includes the basics to get you started with making change requests directly to this repository. If you get stuck, please contact a group member. We'd love to improve the documentation to make it easier for everyone to contribute.

## Practices for Contributing to this Repository

**Setting up a new child site repository**

1. Select the Import Repository Option from the Github site
2. You will be taken to a page that lets you create a new repository based on an existing one. Make sure the owner of the new repository is DLFMetadataAssessment. For the text box titled "Your old repository's clone URL" input ```https://github.com/DLFMetadataAssessment/EnvironmentalScan.git```. This is the URL for the EnvironmentalScan child repository.
3. Delete the content of the entries folder. You will repopulate this folder with content of your new child repository.
4. Modify ReadMe.md as needed to describe your new child repository.
5. Modify Index.md as needed to describe your new child repository.
6. Modify includes/nav.html. You will need to remove the links to the Environmental Scan child repository and add links to your new repository and any new content in the entries folder. Your new repository can be linked as the root page ```/```. Put any pages in the entries folder you create in an unordered list under the link to your new repository. The links to these will follow the format ```/entries/filename.html``` where "filename" is the file name of the page you are linking to.

**Branch Names**

Once an issue is raised in our GitHub repository, we create a branch with a name based on the issue number it is addressing, i.e. 'issue#1'. The pull request generated to fix Issue 1 is then the merging of that branch into the **master** branch, which feeds into the Github.io website.

You can see and comment on a list of [outstanding issues](https://github.com/DLFMetadataAssessment/DLFMetadataAssessment.github.io/issues).

The examples and walk through of GitHub and Jekyll below uses "issue#3" as a subject. That's the branch name used in the commit message.

**Pull Requests**

Once you have committed your changes to your branch for a particular issue, submit a pull request to have your changes reviewed. It will be merged by another member of the group. We request that nobody merges their own pull requests.

If your pull request sits for a while, you can submit an email to the [Google Group](https://groups.google.com/forum/#!forum/dlf-aig-metadata-assessment-working-group) asking for it to be reviewed.

### About GitHub

If you're new to GitHub, we recommend an [introduction to the GitHub flow](https://guides.github.com/introduction/flow/) and [simple steps for getting started in GitHub](https://guides.github.com/activities/hello-world/).

### About Jekyll

This site is built with Jekyll. [Jekyll](http://jekyllrb.com) is a Rails gem that generates static websites from markdown, HTML, and other formats. See the [official Jekyll documentation](http://jekyllrb.com/docs/home/) for details and instructions on how to install. There is also a comprehensive guide to installing Jekyll on a Windows machine available [here](http://jekyll-windows.juthilo.com/).

### Here's how to make a Git Pull Request for this Jekyll site:

#### The first time you want to contribute

You'll need:

1. Git
2. Ruby version between 2.0 and 2.2
3. Rubygems
4. Bundler
5. Jekyll

In a terminal:

1. clone the repo with ```git clone https://github.com/DLFMetadataAssessment/DLFMetadataAssessment.github.io.git```
2. change to the repository's root directory with ```cd DLFMetadataAssessment.github.io```  
3. run ```bundle install```
4. Continue with step 3 below

#### Subsequent work
1. Make sure you're on the master branch (necessary if you skipped step 9): ```git checkout master```
2. Make sure your master branch is up to date: ```git pull origin master```
3. Start up jekyll: ```bundle exec jekyll serve``` then check [http://localhost:4000](http://localhost:4000)
4. create a new branch for your changes: ```git checkout -b issue#3```
5. make changes, check [http://localhost:4000](http://localhost:4000) to see your changes
6. add your changed files: ```git add {changed-files}``` or ```git add .``` to add all untracked files
7. commit your changes with a message: ```git commit -m "fixes issue #3"```
8. add your branch to the repo: ```git push --set-upstream origin issue#3```
9. switch back to the master branch: ```git checkout master```
10. go to https://github.com/DLFMetadataAssessment/DLFMetadataAssessment.github.io/pulls
11. make a new pull request with base:master and compare:issue-3
12. wait for someone to test your changes and merge (please do not merge your own PRs)
13. start over with step 1 for your next change
