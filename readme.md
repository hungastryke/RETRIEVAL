####**RETRIEVAL - A responsive design jquery search plugin**
[[ View Demo ]](http://hungastryke.com/samples/retrieval)<br />

**A. Description**<br />
This plugin allows you to do search for data immediately as you type into your search field. 

**B. Requirements**<br />
You'll need to download both the [retrieval.css](retrieval.css) and the [retrieval.min.js](retrieval.min.js) from this repository. I recommend placing your [retrieval.css](retrieval.css) file at the base of the head tag. For optimal performance, you should place the [retrieval.min.js](retrieval.min.js) file at the base of your document right before the closing body tag.

**C. How to use**<br />
Retrieval uses the jquery library and as such, uses very similar syntax. If you've used jquery before you should be accustomed to using this tool.

There are two types of dropdowns: one with images and one without. You can view the [demo here](http://hungastryke.com/samples/retrieval).

Here's how it works:<br />

$(**SOME_ELEMENT**).retrieval(function(){<br />
  **search**: $(this),<br />
  **posturl**: AJAX_POST_URL,<br />
  **datatype**: 'json',<br />
  **type**: 'get',<br />
  **key**: 'value',<br />
  **image**: true,<br />
  **imagenode**: NAME_OF_IMAGE_NODE,<br />
  **datanode**: NAME_OF_DATA_NODE_TO_RETRIEVE<br />
});

**search**: this is the input field you're using<br />
**posturl**: url you're using for AJAX url field<br />
**datatype**: this can be json or xml. if field is undefined it'll default to json<br />
**type**: this field is optional. if undefined it'll return as "GET"<br />
**key**: this is the data to be sent to the server<br />
**image**: boolean value. if true you'll need to add a value for the imagenode. if false, you've chosen to use imageless dropdown<br />
**imagenode**: name of the image's key attribute in the datatype<br />
**datanode**: name of the data's key attribute in the datatype<br />

