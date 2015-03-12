# node-ndl-search
a JavaScript library to use NDL Search API by National Diet Library, Japan.

# Usage

ndl = require('node-ndl-search');

ndl.search({isbn:'9784062689007'}, function(json){
  // translated JSON data from XML result of the API call
  console.log(json);
});


Then calls NDL Search API internally; 'http://iss.ndl.go.jp/api/sru?operation=searchRetrieve&query=isbn='+isbn

http://iss.ndl.go.jp/
