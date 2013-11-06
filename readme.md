RETRIEVAL
A responsive design jquery search plugin

A. Description
This plugin allows you to do search for data immediately as you type into your search field. 

B. Requirements
You'll need to download both the retrieval.css and the retrieval.min.js from this repository and an <input /> tag. I recommend placing your retrieval.css file at the base of the <head /> tag. For optimal performance, you should place the retrieval.min.js file at the base of your document right before the closing <body /> tag.

C. How to use
Retrieval uses the jquery library and as such, uses very similar syntax. If you've used jquery before you should be accustomed to using this tool.

There are two types of dropdowns: one with images and one without. Here's how it works:

$(SOME_ELEMENT).retrieval(function(){
  search: $(this),
  posturl: AJAX_POST_URL,
  datatype: 'json',
  type: 'get',
  key: 'value',
  image: true
  imagenode: NAME_OF_IMAGE_NODE,
  datanode: NAME_OF_DATA_NODE_TO_RETRIEVE
});

search: this is the <input /> field you're using
posturl: url you're using for AJAX url field
datatype: this can be json or xml. if field is undefined it'll default to json.
type: this field is optional. if undefined it'll return as "GET"
key: this is the data to be sent to the server
image: boolean value. if true you'll need to add a value for the imagenode. if false, you've chosen to use imageless dropdown
imagenode: name of the image's key attribute in the datatype
datanode: name of the data's key attribute in the datatype

