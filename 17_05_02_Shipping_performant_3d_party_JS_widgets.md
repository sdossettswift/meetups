# Shipping Performant 3rd Party JS Widgets
## SpaceCity.jS
- May 2, 2017
- Iron Yard

 * Caroline Dikibo - People's Choice Award for NASA Hackathon - EmberAlert - alerts you to fires.
 * Next month: Chris will give talk re: Clojure && rum - May 25 
 * Toptal roadtrip - May 25 they will be in Houston 

 @chaddonohue
 @ericclemmons 
 @poeticninja (saul)


3d party perfomant widgets: twitter buttons, chat windows, etc. 

- simple integration - merely a script tag that looks for a signature 

- average SPA ships 420kb js, spends 5s in startup.. Parse time - often overlooked
## HOW TO SPEED UP WIDGETS (w/ minimal effort)

### Stack 
- babel
- webpack
- https://github.com/th0r/webpack-bundle-analyzer (visualization of the code you are shipping- shows you where to cut fat)
- yarn (much!!) faster than npm  (example: 2.5 mins in npm, 20 seconds w/ yarn)
### Example: widgets.js (2.1 mb)

### webpack -p (427kb)
- automatically minifis using uglifyJS
- shims process.env.NODE_ENV = "production" for dead-code removal 
* uglify js will ignore all the development/test stuff that isn't useful for production 
https://webpack.js.org/
- 
### Compression-webpack-plugin (134kb)
- configurable, compressed bundles w/ Gzip
- https://github.com/webpack-contrib/compression-webpack-plugin
`` plugins: [
	new CompressionPlugin({
	test: /\.(html|js)$/
	})
	]
``
### Tree Shaking (109kB)
- babel-plugin-lodash
- tree shaking bundles hte named imports vs. an entire CommonJS module
- https://webpck.js.org/guides/tree-shaking 

### Preact (71.2kB)
- preact-compat is a drop-in replacement for react 
- use webpack's resolve.alias
- current version 8
- there were issues w/ preact 7
- changes dom renderer, changes differ - whole encihilada
- compatability layer
- big preformance improvement, non-technical users will appreciate the ∆
`` resolve: {
	alias:{
		react: "preact-compat",
		"react-dom": "preact-compat"
	}
}``

### Code Splitting (31kb for widgets.js)
- automatically splits dynamic imports 
- built in webpack 

### Targeted Polyfills (6.54kB)
- bundle and ship code to majority of your users based on their browser stats
- lazy-load additional polyfills for uncommon browser targets
- this makes performance super quick for super users w/ most up to date tech 
- figure out what browsers have marketshare 
- ship to chrome first... 
- https://github.com/zloirock/core-js 


chat.js (40.8kB)
hello.js (7.82kB)
polyfills.js(17kB)
widgets.js(6.54kB)
