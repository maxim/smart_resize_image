#PHP - smart&easy image resize function

* resizing an image with 1 simple function.
* more stuff - visit my blog : www.nimrodstech.com

##How to use : (code snippet)

```php
      //indicate which file to resize (can be any type jpg/png/gif/etc...)
      $file = 'your_path_to_file/file.png';
      
      //indicate the path and name for the new resized file
      $resizedFile = 'your_path_to_file/resizedFile.png';
      
      //call the function (when passing path to pic)
      smart_resize_image($file , null, SET_YOUR_WIDTH , SET_YOUR_HIGHT , false , $resizedFile , false , false ,100 );
      //call the function (when passing pic as string)
      smart_resize_image(null , file_get_contents($file), SET_YOUR_WIDTH , SET_YOUR_HIGHT , false , $resizedFile , false , false ,100 );
      
      //done!
```

##Funcion call (with doc)

```php
   /**
   * easy image resize function
   * @param $file - file name to resize
   * @param $string - The image data as a string, default is null
   * @param $width - new image width
   * @param $height - new image height
   * @param $proportional - keep image proportional, default is no
   * @param $output - name of the new file (include path if needed)
   * @param $delete_original - if true the original image will be deleted
   * @param $use_linux_commands - if set to true will use "rm" to delete the image, if false will use PHP unlink
   * @param $quality - enter 1-100 (100 is best quality) default is 100
   * @return boolean|resource
   */
  function smart_resize_image($file,
                              $string = null,
                              $width = 0,
                              $height = 0,
                              $proportional = false,
                              $output = 'file',
                              $delete_original = true,
                              $use_linux_commands = false,
   $quality = 100
   ) {code code code...
   
 ```  
 
### Thanks for all the people adding more functions! keep it going

### Enjoy!






#####License

Copyright © 2008 Maxim Chernyak

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
   
