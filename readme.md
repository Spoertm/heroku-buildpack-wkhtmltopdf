# Heroku Buildpack: wkhtmltopdf

This was made for private use for a program hosted on Heroku.

Edits made:
* Keep wkhtmltoimage and remove wkhtmltopdf
* Use `bionic_amd64.deb` instead of `focal_amd64.deb`
* Output folder changed to `$BUILD_DIR/bin/heroku_output` instead of `$BUILD_DIR/bin`

---

Downloads wkhtmlto* binaries, then copies bin/

## Tested against following

- wkhtmltopdf 0.12.6 r1

## Usage

```
$ heroku buildpacks:set https://github.com/serviceyear/heroku-buildpack-wkhtmltopdf

$ git commit --allow-empty
$ git push heroku

$ heroku run bin/wkhtmltopdf -V

# profit!
```

## Reference

[Heroku Buildpacks](https://devcenter.heroku.com/articles/buildpacks)
