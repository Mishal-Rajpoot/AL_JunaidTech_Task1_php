# AL_JunaidTech_Task1_php
PHP Tasks may include developing applications, writing scripts for data processing, creating  dynamic content, or building APIs.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Internship task 1</title>
</head>
<body>
<?php
$name = "Mishal";
$gender = "Female";
$age = 24;
$address = "123 Main Street,Okara";
$degree = "Bachelor of Science in Computer Science";
$email = "mish@example.com";
$phone = "1234567890";
echo "<h1>Personal Information</h1>";
echo "<p><strong>Name:</strong> $name</p>";
echo "<p><strong>Gender:</strong> $gender</p>";
echo "<p><strong>Age:</strong> $age years old</p>";
echo "<p><strong>Address:</strong> $address</p>";
echo "<p><strong>Degree:</strong> $degree</p>";
echo "<p><strong>Email:</strong> $email</p>";
echo "<p><strong>Phone:</strong> $phone</p>";
?>
    
    <h3>Write a PHP script that demonstrates variable juggling. Hint (Declared Two 
Variable and Assigned them the numeric Value Swap the Value using temporary 
variable. Display the Value before and After Swapping)<br></h3>
<?php
// Declare two variables and assign them numeric values
$a = 20;
$b = 10;
// Display the values before swapping
echo "Before swapping:<br>";
echo "a = $a<br>";
echo "b = $b<br>";
// Swap the values using a temporary variable
$temp = $a;
$a = $b;
$b = $temp;
// Display the values after swapping
echo "After swapping:<br>";
echo "a = $a<br>";
echo "b = $b<br>";
?>
Explanation:
Two variables $a and $b are declared and assigned the numeric values 20 and 10, respectively.<br>
Before swapping, the values are displayed using echo.<br>
A temporary variable $temp is used to hold the value of $a, then $a is assigned the value of $b, and finally $b is assigned the value stored in $temp.<br>
After the swap, the updated values of $a and $b are displayed.<br>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
<h3>3.Declared a Variable With different Data Types and print using gettype and 
var_dump display along variable with data types.</h3><br>
<?php
// Declare variables with different data types
$integerVar = 42;                  // Integer
$floatVar = 3.14;                  // Float (double)
$stringVar = "Hello, world!";      // String
$boolVar = true;                   // Boolean
$arrayVar = array(1, 2, 3, 4);     // Array
$nullVar = null."<br>";                  // NULL
// echo "Integer=$integerVar <br>"  ;
// echo "Float (double)=$floatVar <br>";                  
// echo "String=$stringVar <br>";
// echo "Boolean=$boolVar <br>";
// echo "Arrayy=$arrayVar = array(1, 2, 3, 4)";
// echo "NULL=$nullVar <br>";  

// Display the values and data types using gettype()
echo "<h4>Using gettype():</h4><br>";
echo "integerVar: " . gettype($integerVar) . "<br>";
echo "floatVar: " . gettype($floatVar) . "<br>";
echo "stringVar: " . gettype($stringVar) . "<br>";
echo "boolVar: " . gettype($boolVar) . "<br>";
echo "arrayVar: " . gettype($arrayVar) . "<br>";
echo "nullVar: " . gettype($nullVar) . "<br>";

// Display the values and data types using var_dump()
echo "<h4>Using var_dump():</h4><br>";
var_dump($integerVar);
var_dump($floatVar)."<br>";
var_dump($stringVar)."<br>";
var_dump($boolVar)."<br>";
var_dump($arrayVar)."<br>";
var_dump($nullVar)."<br>";
?>


Explanation of var_dump() output:
int(42) means that the value is an integer (42).
float(3.14) indicates the value is a floating-point number (3.14).
string(13) means the string "Hello, world!" has 13 characters.
bool(true) shows a boolean with the value true.
The array has four elements with values 1, 2, 3, and 4.
NULL is the value of the $nullVar.

<h3>4.Write a PHP script using two variables and perform the following operations Addition, Subtraction, 
Multiplication, Division, Modulo</h3>
<?php
// Declare two variables with numeric values
$num1 = 5;
$num2 = 5;

// Perform Addition
$addition = $num1 + $num2;

// Perform Subtraction
$subtraction = $num1 - $num2;

// Perform Multiplication
$multiplication = $num1 * $num2;

// Perform Division
$division = $num1 / $num2;

// Perform Modulo (remainder of division)
$modulo = $num1 % $num2;

// Display results
echo "Addition: $num1 + $num2 = $addition<br>";
echo "Subtraction: $num1 - $num2 = $subtraction<br>";
echo "Multiplication: $num1 * $num2 = $multiplication<br>";
echo "Division: $num1 / $num2 = $division<br>";
echo "Modulo: $num1 % $num2 = $modulo<br>";
?>
Explanation:
Addition: Adds the two numbers ($num1 + $num2).
Subtraction: Subtracts $num2 from $num1 ($num1 - $num2).
Multiplication: Multiplies the two numbers ($num1 * $num2).
Division: Divides $num1 by $num2 ($num1 / $num2), which gives the result in floating-point.
Modulo: Returns the remainder when $num1 is divided by $num2 ($num1 % $num2).
<br>

<h4>5.using Two Numerical Variables and Write a PHP Scripts to Compare them using Comparison 
Operators</h4>

<?php
// Declare two numerical variables
$num1 = 10;
$num2 = 20;

// Compare the variables using comparison operators

// Equal to (==)
$isEqual = $num1 == $num2;

// Not equal to (!=)
$isNotEqual = $num1 != $num2;

// Greater than (>)
$isGreaterThan = $num1 > $num2;

// Less than (<)
$isLessThan = $num1 < $num2;

// Greater than or equal to (>=)
$isGreaterThanOrEqual = $num1 >= $num2;

// Less than or equal to (<=)
$isLessThanOrEqual = $num1 <= $num2;

// Display the results
echo "Comparing $num1 and $num2:<br>";
echo "$num1 == $num2: " . ($isEqual ? 'True' : 'False') . "<br>";
echo "$num1 != $num2: " . ($isNotEqual ? 'True' : 'False') . "<br>\n";
echo "$num1 > $num2: " . ($isGreaterThan ? 'True' : 'False') . "<br>\n";
echo "$num1 < $num2: " . ($isLessThan ? 'True' : 'False') . "<br>\n";
echo "$num1 >= $num2: " . ($isGreaterThanOrEqual ? 'True' : 'False') . "<br>\n";
echo "$num1 <= $num2: " . ($isLessThanOrEqual ? 'True' : 'False') . "<br>\n";
?>
Explanation:<br>
Equal to (==): Checks if the values are equal.<br>
Not equal to (!=): Checks if the values are not equal.<br>
Greater than (>): Checks if the first number is greater than the second.<br>
Less than (<): Checks if the first number is less than the second.<br>
Greater than or equal to (>=): Checks if the first number is greater than or equal to the second.<br>
Less than or equal to (<=): Checks if the first number is less than or equal to the second.<br>
The script prints "True" or "False" based on the result of each comparison.<br>
<h4>6.. Write a PHP script that demonstrates the use of assignment operators.</h4>
<?php

$number = 10;

// Demonstrate the use of the basic assignment operator (=)
echo "Initial value of number: $number<br>";

// Use the addition assignment operator (+=)
$number += 5;  // Equivalent to $number = $number + 5
echo "After addition assignment (+=5): $number<br>";

// Use the subtraction assignment operator (-=)
$number -= 3;  // Equivalent to $number = $number - 3
echo "After subtraction assignment (-=3): $number<br>";

// Use the multiplication assignment operator (*=)
$number *= 2;  // Equivalent to $number = $number * 2
echo "After multiplication assignment (*=2): $number<br>";

// Use the division assignment operator (/=)
$number /= 4;  // Equivalent to $number = $number / 4
echo "After division assignment (/=4): $number<br>";

// Use the modulus assignment operator (%=)
$number %= 3;  // Equivalent to $number = $number % 3
echo "After modulus assignment (%=3): $number<br>";

// Use the exponentiation assignment operator (**=) (PHP 5.6+)
$number **= 2;  // Equivalent to $number = $number ** 2 (raises $number to the power of 2)
echo "After exponentiation assignment (**=2): $number<br>";
?>


<h4>7.write a PHP script to demonstrate the use of logical operators. Your script should <br>
perform the following tasks: <br>
 Define Boolean Variables:<br>
 Evaluate Logical Conditions:<br>
 Output the Results:<br>

Certainly! Below is a PHP script that demonstrates the use of logical operators. The script defines boolean variables, evaluates logical conditions using AND, OR, and NOT operators, and outputs the results.
</h4>
<?php
// Define Boolean variables
$isRaining = true;
$isWeekend = false;
$isHoliday = true;

// Evaluate logical conditions using logical operators

// AND operator (&&) - both conditions must be true
$canGoToPark = $isWeekend && !$isRaining;  // It's the weekend and it's not raining
// OR operator (||) - at least one condition must be true
$canWatchMovie = $isWeekend || $isHoliday;  // It's the weekend or it's a holiday
// NOT operator (!) - negates the condition
$shouldWork = !$isHoliday;  // It's not a holiday, so I should work

// Output the results
echo "Can I go to the park? " . ($canGoToPark ? "Yes" : "No") . "<br>";
echo "Can I watch a movie? " . ($canWatchMovie ? "Yes" : "No") . "<br>";
echo "Should I work? " . ($shouldWork ? "Yes" : "No") . "<br>";

// Additional logical conditions

// AND with multiple conditions
$canAttendMeeting = $isHoliday && !$isRaining;  // It's a holiday but it's not raining
echo "Can I attend the meeting? " . ($canAttendMeeting ? "Yes" : "No") . "<br>";

// OR with negation
$canRelax = !$isRaining || $isHoliday;  // It's not raining, or it's a holiday
echo "Can I relax today? " . ($canRelax ? "Yes" : "No") . "<br>";
?>
Explanation:<br>
Boolean Variables:

$isRaining, $isWeekend, and $isHoliday are Boolean variables that hold true or false values.<br>
Logical Operators:<br>

AND (&&): Returns true if both conditions are true. For example, if it's the weekend and it's not raining, I can go to the park.<br>
OR (||): Returns true if at least one condition is true. For example, I can watch a movie if it's the weekend or it's a holiday.<br>
NOT (!): Negates the condition. If it's not a holiday, I should work.<br>
The script evaluates the conditions and outputs "Yes" or "No" based on the result of each logical expression.<br>


</body>
</html>
