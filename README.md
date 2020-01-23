# PHP Syntax Guide
PHP Syntax guide/ reference


## PHP Comments ##

A comment in php is used to note out or refer information for code present. This stops any text or code from running in your document 

Syntax:

    // 
    # these two comments need the symbol at the front followed by text
    
    /* this comment has symbols on either side of the text */

Examples:

    // this is a single line comment 
    # this is also a single line comment 
    
    /* this is a 
    multi 
    line 
    comment */ 
    
## PHP Variables ##

A php variable can store information from an input or be declared.

Syntax: 
  
    $any_name_for_your_variable = the content of the variable

Examples:

    $text = "Hello World!";
    
## PHP Echo/Print ##

Echo and Print kind of work the same that you put a variable or text after it and it will display on your page. But syntactically their different. While echo has no value and can have multiple parameters, print has a value of one and can have one parameter.

Syntax echo

    echo "echo comes first with some text or variable behind it";
    echo $this-is-a-variable;
    
Syntax print 

    print "same syntax as echo";
    print $variable-also-the-same;

#### Example echo ####

    $txt1 = 'Hello World!";
    
    echo $txt1;
    echo "What is your name?";
    
#### Example print ####

    $txt2 = "Hello";
    
    print $txt2 . "World";
    print "some more text"
    
## PHP Data Types ##

There are certain data types that php will store in variables. These data types all have different results.

- String
- Integer
- Float
- Boolean
- Array 
- Object
- NULL

### PHP String ###

A string is a sentence or group of characters. You can use double or single quotes to write a string.

#### Example ####

    $var1 = 'Some text';
    $var2 = "Hello World";
    
### PHP Integer ###

An integer can be any number between -2,147,483,648 and 2,147,483,648 without decimals.

#### Example ####

    $var = 3;
    var_dump($var);
    
    //  output int(3)

### PHP Float ###

A float is a integer or number with a decimal point.

#### Example ####

    $var = 30.685;  
    var_dump($var);
    
    //  output float(340.6854)
    
### PHP Boolean ###

A boolean value is either TRUE or False 

#### Example ####

    $x = true;
    $y = false;
    
### PHP Array ###

An array can store infinite ammout of strings or variables. 

#### Example ####

    $cars = array("Volvo","BMW","Toyota");
    var_dump($cars);
    
    //ouput array(3) {[0]=> string(5) "Volvo" [1]=> string(3) "BMW" [2]=>string(6) "Toyota"}
    
### PHP Object ###

An object stores data on how to proccess parameters inputed to that object.

#### Example ####

    //  the constructor for the car object
    class car {
        function car() {
            $this->model = "VW";
        }
    }
    
    //  creating a object in the variable herbie
    $herbie = new car();
    
    //   show an object properties
    echo $herbie->model
    
### PHP Null ###

Null represents a variable with no value which whould be automatically asssigned when the variable is empty.

#### Example ####

    $x = null;
    var_dump($x);
    

## PHP Strings

A string is group of characters in a sentance. A string is writen with quotes either single or double.

### Manipulating PHP Strings ###
    
### Calculating the length of a string ###

To calculation the lenght of the string in number of characters you use the srtlen() function.

#### Example ####

    echo strlen("Hello World!");   
    
    $x = "Hello World!";
    echo strlen($x);    // both outputs 
    
### Counting the words in a string ###

To get the word count in a string we use str_word_count().

#### Example ####

    echo str_word_count("Hello World!"); // outputs 2
    
### Replacing text in a string ###

To replace certain parts of a string with another you can use str_replace() to search the string for a value then replace that value. 

Syntax  str_replace( search-value(string), replacement(string), the-search-string(string) )

#### Example ####

    echo str_replace("world", "bob", "Hello world!"); // outputs Hello bob!
    
### Reversing a string ###

To reverse a string completely you can use the strrev() function.

#### Example ####

    echo strrev("Hello world!"); //outputs !dlrow olleH
    
## PHP Numbers ##

### Infinity ###

Infinity is a value given for a number that has exceeded the float max_size.

#### Examples ####

    $x =1.9e411;
    var_dump($x); //outputs float(INF)
    
### NAN ###

NAN is the value that is given when a mathematical operation cannot be completed. 

    $x = acos(8);
    var_dump($x); //outputs float(NAN)
    
## PHP Constants ## 

Constants are like a php variable that does not change, this means the variables cannot be redefined or incremented in any way.

A best practice when writing constants is to leave them in all caps just to define them better.

There are required parameters name and value but case insensitive is not required and the default is false.

Syntax  define(name, value, case-insensitive)

## PHP Operators ##

### Arithmitic Operators ###

Arithmitic operators are used to perform basic math operations.

| Operator | Description | Example |
|----------|-------------|---------|
|    \+     | Addition    | $x + $y, sum of $x and $y |
|    \-     | Subtraction | $x - $y, difference of $x and $y |
|    \*     | Multiplication | $x * $y, product of $x and $y |
|    \/     | Division    | $x / $y, quotient of $x and $y |
|    \%     | Modules     | $x % $y, remainder of $x divided by $y |

### Assignment Operators ###

Assignment operators are different ways to assign variables.

| Operator | Description | Example | 
|----------|-------------|---------|
|   \=      | Assign      | $x \= $y, $x \= $y |
|   \+=     | Add and Assign | $x \+= $y, $x \= $x \+ $y |
|   \-=     | Subtract and Assign | $x \-= $y, $x \= $x \- $y |
|   \*=     | Multiply and assign |$x \*= $y, $x \= $x \* $y |
|   \/=     | Divide and assign quotient |	$x \/= $y, $x \= $x \/ $y |
|   \%=	    | Divide and assign modulus | $x \%= $y, $x \= $x \% $y |
 
 ### Comparison Operators ###
 
 Comparison operators compare to values and return a boolean statement either true or false.
 
| Operator | Description | Example |
|----------|-------------|---------|
|==	|Equal|	$x == $y, True if $x is equal to $y |
|===|Identical|	$x === $y, True if $x is equal to $y, and they are of the same type |
|!=	|Not equal|	$x != $y, True if $x is not equal to $y |
|<>	|Not equal|	$x <> $y, True if $x is not equal to $y |
|!==|Not identical|	$x !== $y, True if $x is not equal to $y, or they are not of the same type |
|<|	Less than|$x < $y, True if $x is less than $y |
|>|	Greater than|$x > $y, True if $x is greater than $y |
|>= | Greater than or equal to | $x >= $y, True if $x is greater than or equal to $y |
|<=	| Less than or equal to |	$x <= $y, True if $x is less than or equal to $y |

### Incrementing and Decrementing Operators ###

Incrementing/Decrementing operators are to increase or decrease the value of a number data type.

| Operator | Description | Example |
|----------|-------------|---------|
|++$x|	Pre-increment|	Increments $x by one, then returns $x|
|$x++|	Post-increment|	Returns $x, then increments $x by one|
|--$x|	Pre-decrement|	Decrements $x by one, then returns $x|
|$x--|	Post-decrement|	Returns $x, then decrements $x by one|

### Logical Operators ###

Logical operators are used to compare two or more boolean statements.

| Operator | Description | Example |
|----------|-------------|---------|
|and|	And|	$x and $y, True if both $x and $y are true |
|or|	Or	|$x or $y, True if either $x or $y is true |
|xor|	Xor	|$x xor $y, True if either $x or $y is true, but not both |
|\&\&|	And	|$x \&\& $y, True if both $x and $y are true |
|\|\||	Or	|$x \|\| $y, True if either $$x or $y is true |
|\! |	Not	|\!$x, True if $x is not true |

### String Operators ###

There are only two string operators and they both have specific use cases.

| Operator | Description | Example |
|----------|-------------|---------|
|.|	   Concatenation|$str1 . $str2, Concatenation of $str1 and $str2 |
|.=|	Concatenation assignment|$str1 .= $str2, Appends the $str2 to the $str1 |

### Array Operators ### 

Array operators are very similar to boolean operators but instead compare arrays.

| Operator | Description | Example |
|----------|-------------|---------|
|+|	Union|$x + $y, Union of $x and $y |
|==|Equality|$x == $y, True if $x and $y have the same key/value pairs |
|===|Identity|$x === $y, True if $x and $y have the same key/value pairs in the same order and of the same types |
|!=|Inequality|$x != $y, True if $x is not equal to $y |
|<>|Inequality|$x <> $y, True if $x is not equal to $y |
|!==|Non-identity|$x !== $y, True if $x is not identical to $y |

## PHP if and else ##

### if Statements ###

An if statement is used to make a check or codition to then run some code if the check was true.

#### Syntax ####

```
if(condition){
    // code to be executed
}
```

#### Examples ####

    $x = 5;
    
    if ($x > 0) {
        $x = $x -1;
        echo "TRUE!";
    }
    
    
    
### if...else Statements ###

Instead of haveing just code to be executed on true were adding some code for else false.

#### Syntax ####

```
if(condition){
    // code to be executed if true
} else {
    // code to be executed else
}
```

#### Examples ####

    $x = 5;
    
    if($x > 10) {
        echo "true";
    } else{
        echo "false";
    }

###  if..elseif..else Statements ###

You can stack for than one if else statement on top each other with elseif over and over again.

#### Syntax ####
```
if(condition){
    // code to be executed
} elseif(condition) {
    // code to be executed
} else {
    code to be executed
}
```

#### Examples ####

    if(false){
        echo "number one";
    } elseif(true) {
        echo "number two";
    } else {
        echo "nothing";
    }

