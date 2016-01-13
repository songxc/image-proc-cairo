# Image Placeholder Generator

## Introduction

#### Dependencies

- [Express](http://expressjs.com/)
- [Cairo](http://cairographics.org/)
- [Node Canvas](https://github.com/Automattic/node-canvas/)
- [AntiModerate - The progressive image loading library for great good!](https://github.com/whackashoe/antimoderate)

#### Demo

Visit after start service.

- Presentation：<http://127.0.0.1:3000/demo/blur/index.html>  
- Generator：<http://127.0.0.1:3000/demo/blur/tool.html>

#### API
    
    url: http://127.0.0.1:3000/blur
    params:
        {String} callback: callback function name. default: empty;
        {String} src: input image url;
        {Integer} size: output image size. default: 30, maximum: 100;
        {Integer} radius: output image blur strength, bigger leads to more blurry. default: 1, maximum: 20;
    data:
        {Boolean} success: status;
        {String} message: status message;
        {String} errMessage: error message;
        {String} src: input image url;
        {String} size: output image size;
        {String} radius: output image blur strength;
        {String} imgDataURL: output image data url（Base64）;


## Deploy

#### Initialize

1. [express](http://expressjs.com/)：``npm install express --save``
2. [express-generator](https://www.npmjs.com/package/express-generator)：``npm install express-generator -g``
3. [yeoman](http://yeoman.io/)：``npm install yo -g``
4. ``yo express``

#### Update

1. Update [Homebrew](http://brew.sh/)：``brew update``
2. Update Software：``brew upgrade``
3. Install wget：``brew install wget``

#### Install

1. [Cairo](http://cairographics.org/)：``brew install pkg-config cairo libpng jpeg giflib``（For Mac）
2. [Canvas](https://www.npmjs.com/package/canvas)：``npm install canvas``
3. [nodemon](https://www.npmjs.com/package/nodemon)：``npm install nodemon -g``
4. ``npm install``

#### Start

``nodemon ./bin/www``


## Reference

> <a href="http://javascript.ruanyifeng.com/nodejs/express.html" target="_blank">Express</a>    
> <a href="https://stackoverflow.com/questions/10692075/which-library-should-i-use-for-server-side-image-manipulation-on-node-js/10717592" target="_blank">Which library should I use for server-side image manipulation on Node.JS?</a>  
> <a href="http://stackoverflow.com/questions/22286900/how-do-i-interact-with-this-file-object-in-a-node-js-stream" target="_blank">How do I interact with this <File> object in a node.js stream?</a>   
