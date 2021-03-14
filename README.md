# abstract-class
<?php 
abstract class Student{
    public $name;
    public $age;
    public function details(){
        echo $this->name. "is" .$this->age.  "years old";
    }

     abstract public function school();
}
class Boy extends Student{
    public function describe(){
        return parent::details(). "And i am a school student";
    }
     public function school(){
        return "i like to make a content video in youtube";
    }
}

$st= new Boy();
$st->name="Hridoy";
$st->age="22";
echo $st->describe();
echo $st->school(); 

?>
