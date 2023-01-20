_This is a very old version of my website, just for archival purposes._

I had trouble building it myself but I got it to work in 2022.

- Install Python packages (there's many of them and quite tricky ones
  like `slugify` vs `python-slugify`, I added `requirements.txt` but after
  already installing these manually).
- I commented out CSS minification because it used deprecated libraries.
- Install `sass`.
- Run `./build.py` or `./build.py release`

## Original description

My personal website.

I created my own build process. Its source code is
under [MIT License](LICENSE.md), while all of [content/](content/) is
under [exclusive copyright](content/LICENSE.md).

Website is hosted live on Github pages,
see [aleshkev.github.io](https://aleshkev.github.io). I might buy myself some
nice custom domain in the future.

The site is statically built into the `a/` folder. I set up an `index.html`
file, which redirects immediately from `https://aleshkev.github.io/`
to `https://aleshkev.github.io/a/`.

To build, simply use `build.py` or `build.py release`. The `release` mode uses
absolute url, while the default uses only relative links (so the changes can be
previewed by simply opening them in the browser). \
The PyCharm project files already have these two configurations.
