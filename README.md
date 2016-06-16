##&lt;elastic-client&gt;

`elastic-client` is an element that makes a connection to an elasticsearch
server via the standard elasticsearch javascript api.  Once a connection is 
established, the client property can be used by other elements in your application
to access the elastic REST api


Example:
```html
<elastic-client
config='{"host": "http://localhost:9200"}'
client="{{esclient}}"></elastic-client>

<elastic-search 
client="[[esclient]]"
index="myindex"
index-type="[[indexType]]"
query-results="{{results}}"></elastic-search>
```

##Prerequisites
* configure elasticsearch server to run unit tests against a live server instance.
* Web Component Tester
* node, npm, bower
* polyserve or polymer_cli to see documentation and demo page



