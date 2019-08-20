# LUGOD Website

This repo holds the codebase and content for the new LUGOD website.

## Contributing

To setup a local copy of the site, first clone this repo:
```
git clone https://github.com/DAVISLUG/lugod.org.git
```

### Docker

To run the site in a Docker container, simply run `docker-compose up`. This should give you a running Jekyll instance on http://localhost:4000/lugod

### Jekyll + Bundler

To run the site via Jekyll in the traditional way, follow the instructions [here](https://jekyllrb.com/docs/) to install  Jekyll and Bunler on your local machine. Then cd to the root of this repository and run `bundle exec jekyll serve --incremental`, and you should have a site running locally at http://localhost:4000/lugod

## Adding Content

### Add A Meeting

To add a new meeting to the site, simply add a row to the `_data/events.csv` file. Make sure to use the proper datetime format or it won't be prcessed correctly (use the other listed items as a reference).

### Markdown

Markdown is supported, so files that end with `.md` will be rendered as HTML by Jekyll.

### Add A Blog Post

To add a new blog post, add it to the `/_posts/` directory. Use existing posts as a reference to ensure proper filename format and [front matter](https://jekyllrb.com/docs/front-matter/).

### Add A New Page

To add a new general page (like an "About Us" page), add it to the `/pages` directory. Adding a file named `newpage.md` to the `/pages` folder will create a new linkable page at the route `example.com/pages/mypage`. To add this page to the navbar, edit the `_includes/nav.html` file and add your new page.
