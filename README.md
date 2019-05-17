# The LUGOD Website

This site runs on Jekyll.

To setup an instance of the site, first clone this repo.

To run via Docker, simply run `docker-compose up`. This should give you a running Jekyll instance on http://0.0.0.0:4000

To run via Jekyll, install Jekyll to your machine and then run `bundle exec jekyll serve --incremental` in this directory.

To add a meeting, add a row to the `_data/events.csv` file. Make sure to use the proper datetime format for Jekyll to process datetime logic for things like the "next upcoming meeting".

To add a new blog post, add it to the `/_posts/` directory and it will show up in the blog. You can use existing posts as a reference for proper filename format and [front matter](https://jekyllrb.com/docs/front-matter/).

Markdown is supported, so files ending with `.md` can be written as Markdown and will be rendered as HTML.

To add a new page, add it to the `/pages` directory. Adding a `mypage.md` file to the `/pages` folder will create a new linkable page at the route `example.com/pages/mypage`.
