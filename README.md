# LUGOD Website

This repo holds the codebase and content for the new LUGOD website.
This code is not yet deployed to production at https://www.lugod.org, but can
be viewed now on github pages at https://davislug.github.io/lugod.org/

## Local Development

If you'd like to contribute changes to the site, it's often useful to run a
copy of the site locally. To do so, first clone this repo
```
git clone https://github.com/DAVISLUG/lugod.org.git
```

### Docker

If you don't have Docker installed, [go get it!](https://docs.docker.com/get-docker/)
along with [docker-compose](https://docs.docker.com/compose/install/).
Once you have these, you can simply run `docker-compose up` and you'll have a
copy of the site running at http://localhost:4000/lugod.org/

### Jekyll + Bundler

If you can't use Docker or prefer not to, you can run the site via Jekyll the old fashioned way.
First, install Jekyll and Bundler by following the [official instructions](https://jekyllrb.com/docs/).
Then, `cd` to the root of this repository and run `bundle exec jekyll serve --incremental`.
You should now have a local site being served at http://localhost:4000/lugod.org/

## Adding Content

Content can be added by cloning this repository, making necessary changes, and pushing your changes back to the repo.
You can also edit files directly via github.com.
Once files are changed, the site is automatically updated via github pages and is viewable at https://davislug.github.io/lugod.org/ (and eventually https://lugod.org)

### A Note on Markdown

This Jekyll instance supports markdown, so it will convert markdown files to HTML pages automatically.
All you need to do is add a file with the `.md` extension, and Jekyll will convert it to an HTML page when serving the site.

### How To Add A Meeting or Event

To add a new meeting to the site, add a row to the `_data/events.csv` file. Make sure to use the proper datetime format, you can use the other rows as a reference.

### How To Add A Blog Post

To add a new blog post, add it to the `/_posts/` directory. Use existing posts as a reference to ensure proper filename format and [front matter](https://jekyllrb.com/docs/front-matter/).

### How To Add A New Page

To add a new top level page (like an "About Us" page), add it to the `/pages` directory.
For example, if you add a file named `newpage.md` to the `/pages` folder, Jekyll will create a new linkable page at the route `lugod.org/pages/mypage`.
To add a page to the navbar, edit the `_includes/nav.html` file and add a link (you can use the other links as a reference).


