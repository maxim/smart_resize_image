= PHP - easy and smart image resize function

resizing a image with 1 simple function.

for more things visit my blog : www.nimrodstech.com

= How to use : (code snippet)


      //indicate which file to resize (can be any type jpg/png/gif/etc...)
      $file = 'your_path_to_file/file.png';
      
      //indicate the path and name for the new resized file
      $resizedFile = 'your_path_to_file/resizedFile.png';
      
      //call the function (when passing path to pic)
      smart_resize_image($file , null, SET_YOUR_WIDTH , SET_YOUR_HIGHT , false , $resizedFile , false , false ,100 );
      //call the function (when passing pic as string)
      smart_resize_image(null , file_get_contents($file), SET_YOUR_WIDTH , SET_YOUR_HIGHT , false , $resizedFile , false , false ,100 );
      
      //done!


= Funcion call (with doc)


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
   
   
   
Thanks for all the people adding more functions! keep it going

= Enjoy!
