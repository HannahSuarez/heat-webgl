<a href="http://hannahsuarez.me/projects/HeatDistortion/demo/index.html" target="_blank"><img src="http://hannahsuarez.me/projects/MISC/heatdistortion.png"></a>

## Introduction

In this example, I am using a free WebGL library to create a menu board that could be used for a small restaurant. 

Please see the demo folder for related files including the images.

## Installing
First, you'll need [node.js](https://nodejs.org/), which includes `npm`. Then, open the project folder on the terminal and run:

`$ npm i`

## Building and running
### Building
`$ npm run build`

### Watching
`$ npm run watch`

### Running
`$ npm run start`
Then open `http://localhost:8080/demo`.

### Watching & Running
`$ npm run start-dev`

...and when you're done...
`$ npm run stop-dev`

## License

Integrate or build upon it for free in your personal or commercial projects. Don't republish, redistribute or sell "as-is".

Read more here: [License](http://tympanus.net/codrops/licensing/)

###STAGE 1: SET UP THE ENVIRONMENT###

On your machine, install NodeJS and make sure that both NodeJS and NPM are up to date. 

Follow the steps outlined in the HeatDistortionEffect readme.md at https://github.com/lbebber/HeatDistortionEffect to build, watch and run the project. This repository includes all of the samples provided to create various heat distortion effects. The cooking heat distortion effect is the example that I've used for this post.

###STAGE 2: TEST ON LOCALHOST###

After following through the steps outlined in the Heat Distortion Effect readme.md to build the project on your own machine, go to the page that you have built on http://localhost:8080/ to view the initial web page. The example that I've used is located at index3.html (the cooking example).

Before making tweaks to the code, I started with the images that I wanted to apply the heat distortion effect to.

###STAGE 3: READY YOUR IMAGES###

Start with one image to see how the effect looks. We'll need to create three instances of the same menu image item for this effect.

Image 1: Original Image

Using the highest resolution available for your photo is recommended. 

This image is a stock photo - you can use your own.

Image 2: The Blurred Image

Duplicate the original image to create its blurred counterpart and further simulate the heat distortion effect. Using the free and open source tool GIMP, I used the Gaussian Blur filter. You can use other filters, settings and image editing software to create the blurred image effect.

After creating the Gaussian Blur effect, I exported to a JPG file at the 100% quality. You may have your own preference or file formats to keep to the highest quality. As long as it works for you!

Image 3: The Heat Map Image

I duplicated the original image to create a 'heat map' type image rendering. This helps further simulate the heat distortion effect.

In GIMP, I reduced the image to three colors via Color > Posterize > selecting to 3 colors only. On a new layer, I added the green-to-white gradient and selected the Layer mode to 'Darken only' meaning that the green will only show on the white areas within the posterized image. 

The heat map image plays a role on where the heat distortion takes place. You may end up doing a few other changes to this, but for the first iteration, let’s see how it will look like when brought together with the rest of the images.

###STAGE 4: REPLACE THE IMAGE ASSETS IN THE JAVASCRIPT CODE###

Once your image assets are ready, save them in the img folder under demo. Replace the uploaded image links in the .js file located at /build/cooking.js

###STAGE 5: TWEAK THE CSS###

If you are planning to do further tweaks to the CSS, you can do so by editing the cooking.css file in demo/css folder

###STAGE 6: TWEAK THE HTML###

You can do any further tweaks to the main HTML page.

###STAGE 7: TWEAK THE IMAGES###

Perhaps there is not enough heat distortion in the final product, there is too little or it's not in the right area. I decided to make a second iteration of the image - tweaking the Gaussian blur and other settings.

Make sure that any image file changes go back to the JS file containing the image assets. 

I tested 'on sight' by refreshing the demo on http://localhost:8080/ until the new change had the desired heat distortion effect that I am looking for.

###STAGE 8: UPLOAD TO YOUR WEB SERVER###

Upload on to your own web server. 