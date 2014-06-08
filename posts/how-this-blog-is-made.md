<!-- 
.. title: How this blog is made
.. slug: how-this-blog-is-made
.. date: 2014-06-08 15:53:51 UTC+01:00
.. tags: static generated sites, github pages, nikola
.. link: 
.. description: An intro to static blogging engines for Github Pages
.. type: text
-->

# How is this site made

So, you may have noticed that there are lots of sites popping up with *.githib.io addresses, and perhaps you've wondered a bit about how you can do this yourself?  Fortunately, it's really simple, it's easy, and it's free.

## Get a Github account

Assuming you haven't already, get a github account.  They come in handy for all manner of things anyway; like collaborating on open-source projects in groups, and version control, and other stuff like that.  Github accounts come with the ability to setup Github pages.

You can find out how to do that at (pages.github.com)[https://pages.github.com/]. Basically, you just create a repository in your github account in this format:

<your-username>.github.io

...and then you clone it and push whatever you want to host to it, but check the guide I linked to, it's much better if you aren't familiar with git.

## Create some content

The content you host on your Github pages account must be static.  There's no server side generation going on.  The simplest version of this is just to upload HTML pages to the site, but you do of course deal with issues if you want to update something on each page - you'd have to edit every HTML page.

As a side note: the best bit about this is that, because it's a git repository, you have versioning on all of it.  It's easy to roll back the entire thing to a previous version.  People can collaborate on it by cloning the respository and creating new commits of their own.

## Consider using a static site generator

Because all content is static, and this can cause headaches if you change site design or want to update every page (say, a 'latest posts' list, which would need to appear on every page.), you should consider using a so-called static-CMS, or static site generator.  The most popular are Jekyll and Octopress, both of which are written in Ruby, but others are available in most languages.

I'm more of a Python guy than Ruby guy, so I use a static generator written in Python called Nikola.  Most generators are written in Ruby, Python or Javascript (usually as a Node.js application) but all sorts are available.  Find a list of static site generators (here)[http://staticsitegenerators.net/] or (here)[http://www.staticgen.com/]

Generators run mostly from command line (there are even a couple written in BASH), and generate sites on command from files you provide in a markup language like HTML, Markdown, ReStructured Text, Textile or one of the others.

## That's it, you're good to go

Once you've installed a site generator, create a git folder in it's output folder, and set it up to push to your repository from earlier.

After you push your first commit, it'll be live.  Go tell the world something.  Making it dev-related might be most appropriate!