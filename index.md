<?php

interface ShapeInterface {
    public function area();
}

class Kategorija {
    public $naziv;
    public $redosled;
    public $link_slike;
    

    public function __construct($naziv,$red,$link) {
        $this->naziv = $naziv;
        $this->redosled = $red;
        $this->link_slike = $link;
    }

    public function get_naziv() {
        return $this->naziv;
    }
    public function get_link_slike() {
        return $this->link_slike;
    }
    
    public function set_naziv($naziv) {
         $this->naziv = $naziv;
       
    }
    public function set_link_slike($link) {
       
        $this->link_slike = $link;
    }
    public function set_redosled($red) {
       
        $this->redosled = $red;
        
    }
}

class Spisak_kategorija {

    protected $vrste;

    public function __construct($vrste = array()) {
        $this->vrste = $vrste;
    }

    public function prikazi_nazive() {
    
    foreach($this->vrste as $vrsta) {
       // if(is_a($shape, 'ShapeInterface')) {
            $nazivi[] = $vrsta->get_naziv();
            echo $vrsta->get_naziv()."<br>";
             echo "<img src='". $vrsta->get_link_slike()."'>";
       //     continue;
       //}
        
    
    }
     return $nazivi;

    }

    public function prikazi_slike() {
    
    foreach($this->vrste as $vrsta) {
       // if(is_a($shape, 'ShapeInterface')) {
            $linkovi[] = $vrsta->daj_sliku_kategorije();
            echo $vrsta->daj_sliku_kategorije()."<br>";
            echo "<img src='". $vrsta->daj_sliku_kategorije()."'>";
       //     continue;
       //}
        
    
    }
    }
}
         


class Prikaz {
    
    protected $imena;
    
    
    public function __construct($imena = array()) {
        $this->imena = $imena;
    }
    
    
    public function prikazi_imena(){
        foreach($this->imena as $ime) {
       // if(is_a($shape, 'ShapeInterface')) {
            echo "<br>".$ime."<br>";
        //    continue;
       //}
        
    
    }
        
    }
}

$kategorije = array(
    
    new Kategorija("Prva",2,"https://scotch-res.cloudinary.com/image/upload/w_1050,q_auto:good,f_auto/media/https://scotch.io/wp-content/uploads/2015/03/solid-object-oriented-design.jpg"),

    
);



$spisak = new Spisak_kategorija($kategorije);

$lista=$spisak->prikazi_nazive();
$lista=$spisak->prikazi_slike();
//$pr= new Prikaz($lista);
