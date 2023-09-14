# oops
oops

oops - things revolve around object program become real world so , it's redability encahnce

class - it is a user defined data type 
object - it is instance of class

keywords
-- THIS - THE ADDRESS OF THE CURRENT OBJECT GOT STORED HERE
class hero{
//properties 
public:
  int health ; 
private:
char car ;

char getcar(){
return car ;}

void setcar(char x){
 car = x ; }

 hero(int health){
 this->health = health ;
  }:

  int main(){
  //creation of object
  hero hi; 
  hi.health = 10 ;
 cout<<hi.getcar();
  cout<<sizeof(hi) ;
   cout<<h1.health ;

   //dynamic allocation 
   hero *a = new hwro() ;
   cout<< a->health ;
   cout<<a->getcar ;
  }
**in case of empty class the memory allocation is of 1 byte
property of object got access through dot operator
  cout<<h1.health ;

--access modifier(by default it's private)
1.private - it can access inside the class only 
2.public - it can access inside and outsid the 

access the private access modifier through geter and seter 

--// dynamic allocation
hero *b = new hero ;

-constructor - when an object got created it got invocted with no rteurn type
when we write hero h1 then hero.h1 constructor got called 
once called at the time o construction of the object
1.default constructor with no parameters 
hero(){
cout<<"constructor call" ; }
2.parametaris constructor
hero(int health){
this->health = health) ; }
3.copy constructor
  pass by value - makethe copy
  pass by reference - make changes then got into original 

---copy things here through
shallow copy - default copy constructor do shallow copy here memory got accessed by different names
deep copy - 

--copy assignment opperator - object created already then you copy through this operator

-distructor - to deallocated the memory we use this , called only once for the object at the time o distruction
for static allocation distructor called autometically but for dynamic allocation distructor had to called manully
~hero(){ cout<< );
*static function - no need to creat object ,this keyword won't be their and static function access static member
static int = h 

//static keyword - 






//4 pillars of oops 
1.encapsulation (info. hiding)- raping the data member AND member function
    class use both data member and member function being declired inside
  fully enpaculated is that where all the data member are marked private
advantages - data hiding by private marking , security inc. ,
      class will be marked read only , managbility

2.inheritance - property of super class got inherit into some other class
         parant class (super class ) -  sub class 

public mode - class child_name : public super_name{
string colour ;
void week(){ cout<< colour.}

else their are private and protected mode

----type of inheritance 
1.single - 
2.multilevel - multiple level pe inheritence
3.multiple - c is a class that inherit onjects from different multiple classes
            class child_name : public parent1_name , public parent2_name {    }
4.hyrarchial - one class parent classes for multiple classes
5.hybrid - combination of more than one type of inheritance

------ambiguty - resolve through scope resolution operator 
      in case of multiple inheritance - we see this when the same name function called from different parant  class
      then to access them we use this operator
    obj.a::func() ;


3. polymorphisum - single action performed in multiple ways
   (i).compile time - in how many different form this intity going to exit
           it has function overloading and 
5. 
java convert into whitegod java virtual machine  , code reuseability

mulyilevel - c - a - b
multiplelevel - more than two paretn for a child 

-nstaatic keywwprd - ek baar hi memeory allocate hoti h first time the class load
                       with object access  memroy saved , public static oid main

- class variable - ek baar memory allocate hogi , ut value can be changed , made through stativ keyword

-incapsulation - data secure through access modifer , hide sensitve data from user
protected parent and theri chid calass use 
private - class inside that method can 
-polymorphisum -same name of function with different arggument
run time (overwritting)- if the function in parant and child class
compile time(overloading) - if both the function inside same class
-abstract = hide the underlying complexity of the system from teh users 
abstract keyword - no need to difine in that parant classes they define in derived class 
