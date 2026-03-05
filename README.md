# Some Basic problem solving in javascript language

## Fibonacci Series

let n = 10;
let a = 0;
let b = 1;

console.log("Fibonacci Series:");
for (let i = 1; i <= n; i++) {
    console.log(a);

    let next = a + b;
    a = b;
    b = next;
}

Logic :
First two numbers get 0 and 1
Next number = previous two numbers ka sum






## Sum of Total Digit in a Number

let num = 1234;
let sum = 0;

while (num > 0) {
    let digit = num % 10;
    sum = sum + digit;
    num = Math.floor(num / 10);
}

console.log("Sum of digits:", sum);

Logic : 
%10 → last digit nikalta hai
/10 → last digit remove karta hai
digits ko sum me add karte hain






## Palindrome Number

let num = 121;
let original = num;
let reverse = 0;

while (num > 0) {
    let digit = num % 10;
    reverse = reverse * 10 + digit;
    num = Math.floor(num / 10);
}

if (original === reverse) {
    console.log("Palindrome Number");
} else {
    console.log("Not Palindrome");
}

Logic : 
number ko reverse karo
agar original == reverse
then Palindrome




## Triangle Pattern

let rows = 5;

for (let i = 1; i <= rows; i++) {

    let pattern = "";

    for (let j = 1; j <= i; j++) {
        pattern += "* ";
    }

    console.log(pattern);
}

Logic : 
outer loop → rows control karta hai
inner loop → stars print karta hai





## Factorial

let num = 5;
let factorial = 1;

for (let i = 1; i <= num; i++) {
    factorial = factorial * i;
}

console.log("Factorial:", factorial);

Logic : 
n! = n × (n-1) × (n-2) × ... × 1
