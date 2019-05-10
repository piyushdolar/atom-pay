# Atompay Integration
Atom payment gateway for PHP or Codeigniter

# Installation
1. Download above library file.
2. Add to your CI library 
3. Load library into your controller.
4. Now call below functions.
5. That's it.

# Call below function from anywhere in your controller
public function __constructor(){
  parent::__constructor();
  $this->load->library('atompay');
}

# Calling atom pay functions.
    public function atom_request(){  
      $this->atompay->atom_request();
    }

    public function atom_response(){
      $v = $this->atompay->atomResponse();
      pre($v);
    }
