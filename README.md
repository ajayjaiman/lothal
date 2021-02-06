# Lothal: A Hugo theme for a responsive blog with hero images

![Lothal theme screenshot](/images/screenshot.png "Screenshot")

## Live demo
[Live demo](https://lothal.netlify.app)

## Key features:
- Fast loading : Lighthouse scores of 90 for mobile and 98 for desktop (last checked on September 28, 2020)
- Fast and responsive website for multiple device sizes
- Hero images for each post (can be disabled)
- Lazy loading, responsive images 
- Multiple shortcodes: for embeded images, youtube videos, netlify contact form...
- Social media icons


## How to get it the theme to work
---
1. Create a themes folder (if it doesn't already exist)
2. Clone the them into the themes directory
```
git clone https://github.com/ajayjaiman/lothal.git
```
You could also downlaod and copy the theme into the themes folder
3. Register the theme in the config folder: theme: lothal

## Managing responsive & lazy loading images and also hero images 
### If deploying through Forestry
- Create a media folder in the content folder 
- Add an _index.md file in it with the following content
```
---
title: Media 
url: "/media"
---
```
- Add the following in the site params
```
  common_media-folder: "media"
```
PS: You can name the media folder "media" or "images" or something else, just remember to change the value in the params

### If 'NOT' deploying through Forestry
You can continue to follow the above method of keeping all mages in one folder or the default Hugo method of keeping images in the post bundle. If you wish to keep the default Hugo bundle remember to comment out common_image_folder param in the params.


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

#### Add the logo file
Add the logo files to the static folder and add details to the config file like this
```
params:
  logo:
      url2x: "/images/lothal-logo@2x.png"
      width2x: 370
      url: "/images/lothal-logo.png"
      width: 185 
```

#### Define up the main sections that you wish to show on the home page
Example of main sections (under params)
```
params:
  mainSections: 
    - "post"
    - "docs"
```

#### Define Google Analytics id in config
```
params:
  google_analytics: "A-RANDOM-ID"
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

If you wish to use the Netlifiy form then define the form name in config file under params
```
params:
 netlify_form: "portlothal"
```

### License
Coder is licensed under the MIT license.

### Maintenance

This theme is maintained by its author [Ajay Jaiman](https://www.jaiman.org)

### Special Thanks

[UIkit](https://github.com/uikit/uikit): a lightweight and modular front-end framework for developing fast and powerful web interfaces.

