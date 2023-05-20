# Explain what a callback function is and provide a simple example

- A callback the function is a function that is passed to another function as an argument and is executed after some operation has been completed. Below is an example of a simple callback function that logs to the console after some operations have been completed.

function modifyArray(arr, callback) {
// do something to arr here
arr.push(100);
// then execute the callback function that was passed
callback();
}

var arr = [1, 2, 3, 4, 5];

modifyArray(arr, function() {
console.log("array has been modified", arr);
});

# OOP

Angular in developed on this concept

# 4 Pillars

encapsulation
abstraction
inheritance
polymorphism

# Procedural programming

Only functions and data seperately

# OOP

- Encapsulation

It combines functions and variables together

let employee ={
baseSalary=5000,
getWage:function(){
return this.baseSalary
}
}

# The best function are those with no parameters

- Abstraction => do not have to worry about working mechanism

# Function Declaration

function fName(){

}

# Function Expression

const fName=function(){

} 
