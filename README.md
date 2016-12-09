# TypeScript

//variables in TS//
1.
var firstname = "neha";
var lastname = "bajare";
var fullname;
fullname = firstname + lastname;
document.body.innerHTML = "fullname" +fullname;

2.
var z;
var y;
var x;
z = 'one';
y = 'two';
x = y + " " + z;
document.body.innerHTML = " " + x 

3.
var x;
var y;
var a;
a = 'nine';
x = 'five';
y = 7;
a = x + y; 
document.body.innerHTML += " " + a;

//function in TS//

function greeter(person:string){
	return "hello," + person;
}
var user = "jane user";
document.body.innerHTML = greeter(user);

//Arrays in TS//

var pet;
var mylist;
pet = ["spot" , "dogy" ,"cat" , " parrot"];
pet.forEach(function(concat)  {
	mylist = mylist + concat + " , ";
});
document.body.innerHTML = "my pets are " + " " + pet;

//Interfaces in TS//

interface Iplant { Genus:string; Species:string; Region:string; Name:string;}
class plant implements Iplant{ Genus:string; Species:string; Region:string; Name:string;}

var myPlant : Iplant = <any>{};
myPlant.Genus = "Malus";
myPlant.Species = "Domestica";
myPlant.Region = "Northern Hemisphere"; 
myPlant.Name = "Orchard Apple";

alert("I have an " + myPlant.Name + "tree. It is of the genus " + myPlant.Genus + 
      " and of the species " + myPlant.Species + ". It is primarly grown in the"+
      myPlant.Region + ".");
