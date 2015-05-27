#PHP - smart&easy image resize function with crop position option

### due to [issue#1](https://github.com/Nimrod007/PHP_image_resize/issues/6).

##How to use : (code snippet)

```php
      //indicate which file to resize (can be any type jpg/png/gif/etc...)
      $file = 'your_path_to_file/file.png';

      //indicate the path and name for the new resized file
      $resizedFile = 'your_path_to_file/resizedFile.png';

      //call the function with crop from top
      smart_resize_image($file , null, SET_YOUR_WIDTH , SET_YOUR_HIGHT , false , $resizedFile , false , false ,100 , true);

      //call the function with crop from center (defualt)
      smart_resize_image(null , file_get_contents($file), SET_YOUR_WIDTH , SET_YOUR_HIGHT , false , $resizedFile , false , false ,100, false);

      //done!
```

##Funcion call (with doc)

```php
/**
 * easy image resize function
 * @param  $file - file name to resize
 * @param  $string - The image data, as a string
 * @param  $width - new image width
 * @param  $height - new image height
 * @param  $proportional - keep image proportional, default is no
 * @param  $output - name of the new file (include path if needed)
 * @param  $delete_original - if true the original image will be deleted
 * @param  $use_linux_commands - if set to true will use "rm" to delete the image, if false will use PHP unlink
 * @param  $quality - enter 1-100 (100 is best quality) default is 100
 * @param  $cropFromTop - if false crop will be from center, if true crop will be from top
 * @return boolean|resource
 */
  function smart_resize_image($file,
                              $string             = null,
                              $width              = 0,
                              $height             = 0,
                              $proportional       = false,
                              $output             = 'file',
                              $delete_original    = true,
                              $use_linux_commands = false,
                              $quality            = 100,
                              $cropFromTop        = false
  		 ) {
   ) {code code code...

 ```  
