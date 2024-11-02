# Jekyll Deployment

```shell
$ bundle exec jekyll build
$ git add .
$ git commit -m "publish"
$ git push origin main
```

For testing I actually don't use live-reload due to some technical problems (mentioned in notes)
```shell
$ bundle exec jekyll build
$ cd _site
$ http-server -- need to install this using node if not exist
```

# Notes

- The value of {{site.url}} should be dynamically changed based on the environment
- the profile picutre is being hardcoded

perhaps this is because I create prefix after the base url
default base url from github pages : `gujarats.github.io`
my base url : `gujarats.github.io/cv/`

## Deployment

This project is using github pages for hosting here is the setup :

- make sure in the setting uses github action
- make sure it uses the static deployment, since I'm going to use different type of statis site generator such as Hugo
- the default path is \_site this is where all the files being deployed to github pages
- see the .github/workflow/static.yml

## Development

Need to change the site.url or remove it from \_config.yaml

# Credits

- I'm using mininal thanks to [orderedlist](https://github.com/orderedlist) for the theme
