# Jekyll Deployment

```shell
$ bundle exec jekyll build
$ git add .
$ git commit -m "publish"
$ git push origin main
```

# Notes

- The value of {{site.url}} should be dynamically changed based on the environment
- the profile picutre is being hardcoded

perhaps this is because I create prefix after the base url
default base url from github pages : `gujarats.github.io`
my base url : `gujarats.github.io/cv/`

## development

Need to change the site.url or remove it from \_config.yaml

# Credits

- I'm using mininal thanks to [orderedlist](https://github.com/orderedlist) for the theme
