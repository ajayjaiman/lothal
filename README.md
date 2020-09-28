# Lothal: A simple and clean blog theme with hero images for Hugo

![Lothal theme screenshot](/images/screenshot.png "Screenshot")

## Live demo
[Live demo](https:/www.x.com)

## How to get it the theme to work
---
1. Copy the lothal folder into the theme folder
2. Register the theme in the config folder: theme: lothal

## Add the features you need in the config file:
---
#### Define the taxonomies that you wis to use
taxonomies example
```
taxonomies:
  category: categories
  tag: tags
  author: authors
```

#### Define the top menu in the config
Menu example: 
```
menu:
  main:
  - name: about
    url: /about/
    weight: -100
  - name: posts
    url: /posts/
    weight: -110
```
#### Define up the main sections that you wish to show on the home page
Example of main sections (under params)
```
params:
  mainSections: 
    - "post"
    - "docs"
```

#### Define the social links in the config
Example of social media links
```
  social:
    - name: facebook
      url: https://facebook.com/xyz  
    - name: youtube
      url: https://youtube.com/xyz
    - name: twitter
      url: https://twitter.com/xyz
    - name: linkedin
      url: https://linkedin.com/xyz
    - name: instagram
      url: https://instagram.com/xyz
```

These are the icons available (please remember to use just this spelling for name):
  - 500px
  - behance
  - dribbble
  - etsy
  - facebook
  - flickr
  - foursquare
  - github
  - github-alt
  - gitter
  - google
  - google-plus
  - instagram
  - joomla
  - linkedin
  - pagekit
  - pinterest
  - reddit
  - soundcloud
  - tripadvisor
  - tumblr
  - twitter
  - uikit
  - vimeo
  - whatsapp
  - wordpress
  - xing
  - yelp
  - youtube


### How to add new posts
Copy the default file in the theme/archetype/defaut.md to the archetype folder in the base of the site

### Add cover image for each post
If you wish to have a cover image for a post you should upload the image in the post folder and type the name of that image in the front matter against 'cover:'
```
title: "Lothal is a Hugo theme"
date: 2020-08-09T16:15:36+05:30
cover: "charles-lebegue-Gaf2DsKoXFU-unsplash.jpg"
description: "This is a test description."
```
### Netlify
This theme can be deployed to Netlify

If you swish to use the Netlifiy form then define the form name in config file under params
```
params:
 netlify_form: "portlothal"
```


### License
Coder is licensed under the MIT license.

### Maintenance

This theme is maintained by its author Ajay Jaiman 

### Special Thanks

[UIkit](https://github.com/uikit/uikit): a lightweight and modular front-end framework for developing fast and powerful web interfaces.

