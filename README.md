# WEBLAB6
Lab Task
1.	Create a function that calulates the power of 100 of a number entered as a parameter.
Code:

function power(x)
    {
        return parseInt(Math.pow(100,x));
    }
  
        let x = 2;
        console.log(power(x));
OUTPUT:  10000
2.	Write a javascript function that takes an array of numbers and a target number. The function should find two different numbers in the array that, when added together, give the target number. For example: answer([1,2,3], 4) should return [1,3].
Code:
var twoSum = function(nums, target) {
    for(let i = 0; i < nums.length; i++){
        for(let j = i+1; j < nums.length; j++){
            if(nums[i] + nums[j] == target){
                return [i, j]
            }
        }
    }
};

console.log(twoSum([15, 7, 11, 2],9))
console.log(twoSum([3, 2, 4],6))
Output: 
[1, 3]
 [1, 2]
3.	Write a javascript function and ask user to enter the age, this function aim to show a message that a person can drive, if the age is greater than or equal to 18 otherwise can’t drive, by using a ternary operator instead of the if-else statement.
Code:

let age = prompt('Please enter your age: ');
let message; 
age >= 16 ? (message = 'You can drive.') : (message = 'You cannot drive.'); 
console.log(message);
 
Output:  You can drive.

4.	Using switch in javascript, write a program to create any four browsers cases of your choice and generate alert (“I am using xyz browser) if user select any one of them.
Code:
var browser= prompt("Select index of the browser you are using: 1.Google chrome, 2. Mozrilla Forefox, 3. Microsoft Edge, 4. Safari");                             
 switch (browser) {
  
  case 1:
    alert( "I am using Google Chrome");
    break;
  case 2:  alert( "I am using Mozrilla FireFox"); break;
  case 3:
    alert( "I am using Microsoft Edge");
    break;
  case 4:  alert( "I am using Safari"); break;
  default:
    alert( "I am using any other browser.");
}
Output:
   
5.	Write a javascript arrow function named calculateSupply that:
a.	takes 2 arguments: age, amount per day.
b.	calculates the amount consumed for rest of the life (based on a constant max age).
c.	outputs the result to the screen like so: "You will need NN to last you until the ripe old age of X"
Code:

  var age = 25;
  var PerDay=500;
  let totalNeeded = (age, numPerDay) => {
  var maxAge = 100;
  var totalNeeded = (numPerDay * 365) * (maxAge - age);
   return 'You will need ' + totalNeeded + ' to last you until the ripe old age of ' + maxAge;;
  }

undefined
totalNeeded()
Output: 'You will need NaN to last you until the ripe old age of 100' 

6. Create an object to hold information on your favorite recipe. It should have properties for title (a string), servings (a number), and ingredients (an array of strings). Write a method “Recipe” that  print the separate lines (one console.log statement for each), log the recipe information so it looks like:
Tea
Serves: 2
Ingredients:
Sugar
Tea
Water
Milk

Code:

const make = {
  Ttile: 'Tea',
  Serving: 2,
  Ingredients: ['sugar', 'tea','water','milk'],
  recipe: function() {
    console.log('Title: ' , this.Title);  
console.log('Serves: ' , this.Serving); 
console.log('Ingredients: ' ,  this.Ingredients);
  }
};
make.recipe()
Output:
Title:  undefined
Serves:  2
Ingredients:   
['sugar', 'tea', 'water', 'milk']

7.	Write a javascript program to get the below object to go from:
let obj = {
  my: 'name',
  is: 'Rudolf',
  the: 'raindeer'
}
// to this:
'my name is Rudolf the raindeer'


Code:

let obj = {
  my: 'name',
  is: 'Rudolf',
  the: 'raindeer',                                                                                                                                                      
 details : function() {
               console.log( "My " + this.my + " is " + this.is , " the " + this.the);
            }
}
undefined
obj.details()
Output:  My name is Rudolf  the raindeer

