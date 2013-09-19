jdf_CI
======

jdf function for codeigniter

install:

1. download `jdf.php` and copy into `libraries` of the `application` folder
2. call `jdf` library and convert time in controller example for `welcome` conroller:
 
      ---------  add code the `index` function in `welcome` controller -------------- 
    $this->load->library('jdf');
    $data['time'] = $this->jdf->jdate('H:i:s P | l, j F Y',time());
    $this->load->view('welcome_message',$data);


    -----------   add code the `welcome_message.php` in `views` folder ---------------
    <?php echo $time; ?>
    

full guide for CI_jdf :

http://seifzadeh.blog.ir/post/CI_jdf

