# oops
oops

Diference between oops and sop(structured priented programming)
oops - things revolve around object + class insted of function program become real world so , it's redability encahnce , reduce redundancy, increase reusability, buttom-top approch , good for data hiding
sop - it provode the logical structuer to program where program is divided funcion, top - bottom appproch , no suppport for data hiding 

class - it is a blue print of object (class = method(function) + attribute(properties))
object - it is instance of class

--Explianing with an example:

class Student:
    name = "nidhi"
# now defineing the instance/object here s1 is the object and student is class 
s1 = Student()
print(s1.name)

**in case of empty class the memory allocation is of 1 byte
property of object got access through dot operator
  cout<<h1.health ;

--access modifier(by default it's private)
1.private - it can access inside the class only 

Class Account:

     def __init__(self , acc_no , act_pas):
            self.__acc_no = acc_no  #become private
            self.__acc_pas = acc_pas   #become private
    
    def reset(self):
       print(self.__acc_pas)
    
acc1 = Account("123456", "asdfgh")
print(acc1.reset()) #no error 
print(acc1.acc_no, acc1.acc_pas)  #show error coz we are calleing rivate attribute them outside the class 
     

2.public - it can access inside and outsid the 

Class Account:
     def __init__(self , acc_no , act_pas):
            self.acc_no = acc_no
            self.acc_pas = acc_pas 
acc1 = Account("123456", "asdfgh")

print(acc1.acc_no, acc1.acc_pas)

access the private access modifier through geter and seter 

--// dynamic allocation
hero *b = new hero ;

-constructor - when an object got created it got iniciated automatically with no rteurn type
when we write hero h1 then hero.h1 constructor got called 
once called at the time o construction of the object
--Defult constructor -
def __init__(self):
      pass 
-- Parametarized constructer
class Student:
  name = "hero"
  def __init__(self , fulname):  
      print(self) #print student
      print("adding student to bd")
      self.name = fulname
 
s1 = student("nidhi")
print(s1.name) #karan

class Student:
  collegename = "hero" #Class attrubute - the instance that are comman for all the object we make class attribute 
  name = "abc" 
  def __init__(self, name, marks):
      print(self) #print student
      print("adding student to bd")
      self.name = name   #instance attribute the instance of the class are differenct 
      self.marks = marks
 def welcome(self):    #mehods
       print("welocome student", self.name)
 def get_marks(self):
      return self.mark  
      
s1 = student("nidhi", 92)
print(s1.name, s1.marks) #karan
s1.welcome()  #print welcome student nidhi
print(s1.get_mak()) #print 92

--IN THE CASE OF SAME CLASS AND INSTANCE ATTRUBUTE THE INSTANCE HAS MORE PRECIDENCE MEAN'S THAT GOT EXECUTED .

--Here SELF is a reference of the current instance of obect 

--Static Method - Methid that doesn't use static parameter(work at class level) 
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

public mode - class child_name : public super_name

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

4.abstraction - implementation hiding 

interfacing can be implemented through sbstesct keyword ehere , abstracted can't be implemented
through interface and abstract key had static ,non static , final and non final variable but interface have only static or ginal variable 



 
