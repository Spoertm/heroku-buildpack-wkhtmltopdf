# Heroku Buildpack: wkhtmltopdf

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
