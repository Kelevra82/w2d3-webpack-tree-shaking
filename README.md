# w2d3-webpack-tree-shaking

My Observations

  Tree Shaking: I exported/imported 3 functions into index.js but didn't use one of them (sayGoodbye). The unused function only shows it being imported from greetings.js in the bundle.js file in development mode and doesn't show up at all in production mode. Also, the size of the bundle.js file is noticably smaller in production mode(~5kb) compared to development mode(~25kb).

  Loader Behavior: I installed the css-loader and style-loader then set the test and use properties in webpack.config.js to load .css files. I made a styles folder in src and created a style.css file in it then imported it in index.js. I launched live server to see if the background color I set in style.css displayed in the browser and it did.