[![Backers on Open Collective](https://opencollective.com/react-pwa/backers/badge.svg)](#backers) [![Sponsors on Open Collective](https://opencollective.com/react-pwa/sponsors/badge.svg)](#sponsors) [![Dependencies Status](https://david-dm.org/Atyantik/react-pwa.svg)](https://david-dm.org/Atyantik/react-pwa)
[![devDependencies Status](https://david-dm.org/Atyantik/react-pwa/dev-status.svg)](https://david-dm.org/Atyantik/react-pwa?type=dev)
[![Build Status](https://travis-ci.org/Atyantik/react-pwa.svg?branch=master)](https://travis-ci.org/Atyantik/react-pwa)
[![Known Vulnerabilities](https://snyk.io/test/github/atyantik/react-pwa/badge.svg)](https://snyk.io/test/github/atyantik/react-pwa)


# React PWA
A highly scalable, Progressive Web Application foundation with the best Developer Experience.

[Watch it in action: Checkout the demo](https://react-pwa.now.sh/)

##### Results
We haven't implemented CDN yet, thus a bit of variation in performance.
###### Chrome Lighthouse
![Lighthouse Performance](https://www.atyantik.com/wp-content/uploads/2017/10/Lighthouse-Performance-Report-React-PWA.png)
Don't go with image, [Check for yourself in your browser](https://developers.google.com/web/tools/lighthouse/)
*We ommited the performance as it was just **82** (pretty good huh??). Cause of server latency. Server is located somewhere in USA and we are in India*  

###### GTMetrix
![GTMetrix Performance](https://www.atyantik.com/wp-content/uploads/2017/10/GTMetrix.png)
Don't go with image, [Check for yourself at GTMetrix](https://gtmetrix.com/reports/react-pwa.now.sh/XLLjOm78)  

###### Pingdom
![Pingdom Performance](https://www.atyantik.com/wp-content/uploads/2017/10/pingdom.png)
Don't go with images, [Check for yourself at Pingdom](https://tools.pingdom.com/#!/YB2qd/https://react-pwa.now.sh)

#### Features
##### Code splitting
The very difficulty faced when developing enterprise application is code splitting. We don't need everything in single JS file. Why not create individual JS files for respective module/page!
We make it really easy here to just create a page that return array of routes. Code is split and loaded automatically when the respective route is called.
*(Enabled in production mode)*  

##### Hot Reloading
Development is lot easy with hot reloading. Make changes and the code is auto/hot-reloaded in the browser.
And we have not missed "sass". Preserver application state when you update in underlying code.  

##### ES6/7 Compatible
Using babel we support the next generation JavaScript syntax including Object/Array destructuring, arrow functions, JSX syntax and more...  

##### Backed by React-Router
We are using the most accepted React router for routing the application. Add your favorite /about, /contact, /dashboard pages.  

##### Offline support
Yes your application is offline available. Run without internet. Pretty cool huh?? Well all thanks to service workers.
*(Enabled in production mode)*  

##### SSR - Server side rendering
The best way to get your application SEO-ed is enable Server side rendering i.e. Universal applications.
*(Enabled in production mode)*  

##### SEO
Our customized routes enable creating meta tags to create Twitter, Google+, Linkedin, Facebook cards. We know how important SEO is to an application.  

##### Content Folding
Show only relevant data when loading via server. Fold your content to save bytes.  


##### Page Caching
Well now you can cache a page in SSR. Pretty simple. just add cache option to route 

`{ cache: { enable: true, duration: 10000}}`
 
this helps you cache page when rendered via server. Why increase server load when page is static and cacheable! 

##### API caching
**Wait what?** Why do you need to cache API ? With service worker & cache mechanisms, even opaque response can be cached (no kidding!).  

##### Webpack ^3.6
We support the latest webpack for best output.  

##### Pre-loading
Preloading for non-html browsers. Yes we give a damn about old browsers.  

##### PWA support (Manifest.json)
Automatic generation of manifest.json. Lets make sure, we look good when someone adds us to home-screen.  
  

##### WebP Support 
Make your application super fast with WebP support. Read more about it at
[https://developers.google.com/speed/webp/](https://developers.google.com/speed/webp/)  

##### Image optimizations
Optimize your images when you create a build. this does slow the build process, but is totally worth it when your site loads fast. We are using imagemin plugins to optimize 
SVG, JPEG, GIF & PNG  

##### PWA - SrcSet Loader (Progressive Image Loading)
Load appropriate srcset and make your site load fast for different view-port devices. We support srcset with WebP out of the box.  

##### HSTS Supported
Enable HSTS for secure sites. Options to define maxAge and preload of HSTS. All with very simple configuration.  
   


### Quick start

- Clone this repo using `git clone --depth=1 https://github.com/Atyantik/react-pwa.git`
- Move to the appropriate directory: `cd react-pwa`.
- Use yarn to install dependencies: `yarn`
- run `yarn start` to see the example app at http://localhost:3003.
- To build the application you should run `yarn build`
- To build and run PWA demo use the command `yarn build && node dist/server.js`  

Now you are all set, Get your hands dirty with this awesome boilerplate.  

### Documentation
*Still in progress... But why don't you checkout our [project's wiki](https://github.com/Atyantik/react-pwa/wiki)*  

### Testing
*We have not written any test cases yet. Yet mocha is all set to test the application we need contributors for the purpose*  

### Docker support
Now easily manage docker-build, given Docker is properly configured and the terminal that is running the nodejs has access to docker command.

##### Working with docker:

`yarn docker:dev:image` 

Will create a development image named "react-pwa" which will be used during application development and running.
If anything new is added to package.json `yarn docker:dev:image` must be rebuild to get the latest nodejs packages

`yarn docker:dev:start`  
will start the application in docker mode.  
 
`yarn docker:prod:build`  
will start the build the application for production  
 
`yarn docker:prod:image`  
will create a docker image that can be deployed easily to any docker-hub and can create production containers  

`yarn docker:prod:start`  
will start the application in production mode, its necessary to create docker:prod:image prior to docker:prod:start  


### Need contributors.


This project exists thanks to all the people who contribute. [[Contribute]](CONTRIBUTING.md).
<a href="graphs/contributors"><img src="https://opencollective.com/react-pwa/contributors.svg?width=890" /></a>

We are actively looking for contributors for testing, and documentation.
Please contact us: admin [at] atyantik.com or contact [at] atyantik.com  

Visit us at [Atyantik Technologies Private Limited](https://www.atyantik.com)

### Backers

Thank you to all our backers! 🙏 [[Become a backer](https://opencollective.com/react-pwa#backer)]

<a href="https://opencollective.com/react-pwa#backers" target="_blank"><img src="https://opencollective.com/react-pwa/backers.svg?width=890"></a>


### Sponsors

Support this project by becoming a sponsor. Your logo will show up here with a link to your website. [[Become a sponsor](https://opencollective.com/react-pwa#sponsor)]

<a href="https://opencollective.com/react-pwa/sponsor/0/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/0/avatar.svg"></a>
<a href="https://opencollective.com/react-pwa/sponsor/1/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/1/avatar.svg"></a>
<a href="https://opencollective.com/react-pwa/sponsor/2/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/2/avatar.svg"></a>
<a href="https://opencollective.com/react-pwa/sponsor/3/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/3/avatar.svg"></a>
<a href="https://opencollective.com/react-pwa/sponsor/4/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/4/avatar.svg"></a>
<a href="https://opencollective.com/react-pwa/sponsor/5/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/5/avatar.svg"></a>
<a href="https://opencollective.com/react-pwa/sponsor/6/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/6/avatar.svg"></a>
<a href="https://opencollective.com/react-pwa/sponsor/7/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/7/avatar.svg"></a>
<a href="https://opencollective.com/react-pwa/sponsor/8/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/8/avatar.svg"></a>
<a href="https://opencollective.com/react-pwa/sponsor/9/website" target="_blank"><img src="https://opencollective.com/react-pwa/sponsor/9/avatar.svg"></a>

### Supporters
##### Browser stack
Thanks to Browser stack we are able to test the PWA nature of application on various mobiles and write automated test cases.  

[![Browser Stack](https://www.atyantik.com/wp-content/uploads/2017/10/Browser-Stack-Logo.png)](https://www.browserstack.com)


### License
This project is licensed under the MIT license, Copyright (c) 2017 Atyantik Technologies Private Limited. For more information see LICENSE.md.  