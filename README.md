# drop-and-drag-files-with-Dropzone.Js
Drop and drag all filetypes with dropzone.js

click the link below for a good video tutorial

https://www.youtube.com/watch?v=839GW_vYnv0

Actual Example

1. Get a CDN of dropzone.css and place it on your header
  https://cdnjs.cloudflare.com/ajax/libs/dropzone/5.5.1/dropzone.css
2. Get a CDN of dropzone.js and place it on your footer
  https://cdnjs.cloudflare.com/ajax/libs/dropzone/5.5.1/dropzone.js

Copy this html code
**************************************************************************************************************************************
    <form action="/upload" method="POST" enctype="multipart/form-data" class="dropzone" id="my-awesome-dropzone">
        {{ csrf_field() }}
    </form>
**************************************************************************************************************************************

and that's all you need to do.


To Configure the dropzone.js
    place your configuration inside of curly bracket
    the properties of configuration you can get on the link below.
    https://www.dropzonejs.com/#config-addRemoveLinks
    
 <script>
      // "myAwesomeDropzone" is the camelized version of the HTML element's ID
      Dropzone.options.myAwesomeDropzone = {
          paramName: "file", // The name that will be used to transfer the file
          maxFilesize: 1, // MB
          addRemoveLinks: true, //add a remove button to each picture upload
      };
  </script>
