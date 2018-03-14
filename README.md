# Projecteuler 1

Question: If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.

Find the sum of all the multiples of 3 or 5 below 1000.

Solution:
var num = [];
var sum = 0;

for (var i = 0; i < 1000; i++){
  if(i%3 === 0 || i%5 === 0){
    num.push(i);
    sum += i;
  }
}
console.log(sum)

So with this one my thought process was that I had to be able to get all the numbers that are mulitples of 3 or 5 and put them some where, so I made an empty array called num. I also needed a place to store my sum when I add all the numbers together, so I made a variable called sum and assigned it the value of 0. Now listing out a 1000 numbers is hard so I decided to make a for loop to loop through all natural numbers from 0 - 999, for(var i = 0; i < 1000; i++). Next what I need to do is get all the numbers that are multiples of 3 or 5, so I made an if statement , if(i%3 === 0 || (or) i%5 === 0). Now that I have all the numbers that I need I want to push those numbers to my array (num) and add them all together, so I did num.push(i); (.push() is a method that pushes to my array). Then I did sum += i , This will add up all the numbers from 0 - 999 that are multiple of 3 or 5. Finally I want to print my result so I have console.log(sum) giving me an answer of 233168.
