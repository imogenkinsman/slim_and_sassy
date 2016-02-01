# Slim and Sassy
A rails-less template for using slim + sass preprocessing via guard.

### Installation
```
git clone https://github.com/jademcgough/slim_and_sassy.git
bundle
```

run with: `bundle exec guard`

### Q & A
**How does this work?**

While guard is running, it will "watch" files and convert them into html and css whenever they change.

Specifically, guard looks in the `scss/` directory for `.scss` files and outputs `.css` files to `styles/`. Likewise, guard
converts `.slim` files in `templates/` to `.html` files in `public`.

**Why isn't a file I added being converted?**

Try restarting guard - this will usually get it to pick up new files it isn't watching.

If that doesn't work, check the extension names of your files. Guard will only watch files that end with `.scss` and `.slim`.
