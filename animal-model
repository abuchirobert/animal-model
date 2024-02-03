/* 
Name: Abuchi Robert
Path: Web3
Task: Model the Animal class and apply four principles of OOP
*/


//Abstraction - This is simply hiding the inner working of a method and showing only the main thing that's needed.
//Inheritance - This is when a class take on the features of another class and can access the properties and methods available in the class it is inherited from.
//Polymorphism - This is when a class inherits from one class but has other features unique to it.
//Encapsulation - This is making the data in a method or property to be private to the class it belongs to. It can be accessed by only a method or property in the same class thats assigned to it.


//Base Class for Animal Kingdom

class Animal {
    constructor(name, coldBlooded){
        this.name = name;
        this.coldBlooded = coldBlooded;
    }

    static hasBackbone = true;

    //Abstraction
    eat(food){
        
        console.log(`Eats ${food}`);
    }

    //Encapsulation
    //This is a private property of the Animal class
    #numberofeye = 2 // this is encapsulation is use. 
    //all the classes of animal in the Animal kingdom has 2 eyes unless for some classes in the Anthropoda phyla
    eye = this.#numberofeye


    //these are public method
    breathing(part){
        console.log(`I breathe using my ${part}`);

    }

    locomotion(way){
        console.log(`I achieve locomotion by ${way}ing`);
    }

   
    //fish - swim
    //amphibians - hop
    //reptile - crawling 
    //avec - flying
    //mammal - walk
    //anthropods - fly


}


// a private method can only be called by another public method in the same class. This is encapsulation.

//There are 6 classes of Animal Kingdom in this program
// Anthropoda
//Fish
//Amphibia
// Reptila
// Avecs
// Mammal

//INHERITANCE
//Anthropoda class inherits the Animal properties and methods
class Anthropoda extends Animal {
    constructor(name, coldBlooded){
        super(name, coldBlooded)
    }

    static hasBackbone = false;

    eat(){
        super.eat('Nectar')
    }

    breathing(){
        super.breathing('lungs');
    }

    locomotion(way){
        super.locomotion('fly');
    }

    

}
   //this is subclass of the Anthropoda class. It show cases polymorphism in use.
    class Spider extends Anthropoda{
        constructor(name, coldBlooded){
            super(name, coldBlooded)
        }

        eye = 8 //an example of polymorphism
    }

class Fish extends Animal{
    constructor(name, coldBlooded){
        super(name, coldBlooded)
    }

    static hasBackbone = true;

    eat(){
        super.eat('Algae')
    }

    breathing(){
        super.breathing('gills');
    }

    locomotion(way){
        super.locomotion('swim');
    }
}


class Amphibia extends Animal{
    constructor(name, coldBlooded){
        super(name, coldBlooded)
    }


    eat(){
        super.eat('Insects')
    }

    breathing(){
        super.breathing('lungs or skin');
    }

    locomotion(way){
        super.locomotion('hop');
    }

    static hasBackbone = true;
}

class Reptila extends Animal{
    constructor(name, coldBlooded){
        super(name, coldBlooded)
    }


    eat(){
        super.eat('Plants')
    }

    breathing(){
        super.breathing('lungs');
    }

    locomotion(way){
        super.locomotion('Crawl');
    }

    static hasBackbone = true;
}

class Avecs extends Animal{
    constructor(name, coldBlooded){
        super(name, coldBlooded)
    }

    eat(){
        super.eat('Grain')
    }

    breathing(){
        super.breathing('lungs');
    }

    locomotion(way){
        super.locomotion('fly');
    }
    static hasBackbone = true;
}

class Mammal extends Animal{
    constructor(name, coldBlooded){
        super(name, coldBlooded)
    }

    eat(){
        super.eat('Rat')
    }

    breathing(){
        super.breathing('lungs');
    }

    locomotion(way){
        super.locomotion('Walk');
    }
    static hasBackbone = true;
}


//In the subclasses of the Animal class, we see how they inherit from the base Animal class and change the features such as food, how they breathe and how they work.


//IMPLEMENTATION

const butterfly = new Anthropoda("Butterfly", true);
//console.log(butterfly.toString());
console.log(`Name: ${butterfly.name}.  \nClass: ${Anthropoda.name}.   \nHas Backbone: ${Anthropoda.hasBackbone}`);
console.log(`Cold Blooded: ${butterfly.coldBlooded}`);
butterfly.eat()
console.log(`Have ${butterfly.eye} eyes`);
butterfly.breathing()
butterfly.locomotion()


const spidey = new Spider("Spidey", true);
console.log(`\nThis is a subclass of the ${Anthropoda.name} class in the Animal Kingdom`)
console.log(`I am a ${spidey.name}, I belong to the ${Spider.name} Class of the ${Anthropoda.name} Animal Kingdom`)
console.log(`I have ${spidey.eye} eyes as a Spider, and it is what makes me special from other classes`);




const fish = new Fish("Baracuda", true);
console.log(`\nName: ${fish.name} \nClass: ${Fish.name} \nHas Backbone: ${Fish.hasBackbone}`);
console.log(`Cold Blooded: ${fish.coldBlooded}`);
fish.eat();
console.log(`Have ${fish.eye} eyes`);
fish.breathing();
fish.locomotion();

const frog = new Amphibia("Frog", true);
console.log(`\nName: ${frog.name} \nClass: ${Amphibia.name} \nHas Backbone: ${Amphibia.hasBackbone}`);
console.log(`Cold Blooded: ${frog.coldBlooded}`);
frog.eat();
console.log(`Have ${frog.eye} eyes`);
frog.breathing();
frog.locomotion();

const turtle = new Reptila("Turtle", true);
console.log(`\nName: ${turtle.name}.  \nClass: ${Reptila.name}.   \nHas Backbone: ${Reptila.hasBackbone}`);
console.log(`Cold Blooded: ${turtle.coldBlooded}`);
turtle.eat()
console.log(`Have ${turtle.eye} eyes`);
turtle.breathing()
turtle.locomotion()

const bird = new Avecs("Bird", false);
console.log(`\nName: ${bird.name}.  \nClass: ${Avecs.name}.   \nHas Backbone: ${Avecs.hasBackbone}`);
console.log(`Cold Blooded: ${bird.coldBlooded}`);
bird.eat()
console.log(`Have ${bird.eye} eyes`);
bird.breathing()
bird.locomotion()

const cat = new Mammal("Cat", false);
console.log(`\nName: ${cat.name}.  \nClass: ${Mammal.name}.   \nHas Backbone: ${Mammal.hasBackbone}`);
console.log(`Cold Blooded: ${cat.coldBlooded}`);
cat.eat()
console.log(`Have ${cat.eye} eyes`);
cat.breathing()
cat.locomotion()
