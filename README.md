## Buddysco.com

#### Hugo Website Creation steps
```
hugo new site buddysco.com
cd buddysco.com
git init
git submodule add git@github.com:StaticMania/portio-hugo.git themes/portio
cp -r themes/portio/exampleSite/* ./
hugo server -t portio
```

### Hugo Github pages deployment
Follow the steps mentioned [here](https://gohugo.io/hosting-and-deployment/hosting-on-github/).