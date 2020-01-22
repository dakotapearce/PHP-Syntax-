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

Examples echo

    $txt1 = 'Hello World!";
    
    echo $txt1;
    echo "What is your name?";
    
Examples print

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

Examples 

    $var1 = 'Some text';
    $var2 = "Hello World";
    
### PHP Integer ###

An integer can be any number between -2,147,483,648 and 2,147,483,648 without decimals.

Examples

    $var = 3;
    var_dump($var);
    
    //  output int(3)

### PHP Float ###

A float is a integer or number with a decimal point.

Examples

    $var = 30.685;  
    var_dump($var);
    
    //  output float(340.6854)
    
### PHP Boolean ###

A boolean value is either TRUE or False 

Examples 

    $x = true;
    $y = false;
    
### PHP Array ###

An array can store infinite ammout of strings or variables. 

Exmples

    $cars = array("Volvo","BMW","Toyota");
    var_dump($cars);
    
    //ouput array(3) {[0]=> string(5) "Volvo" [1]=> string(3) "BMW" [2]=>string(6) "Toyota"}
    
### PHP Object ###

An object stores data on how to proccess parameters inputed to that object.

Example

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

Examples

    $x = null;
    var_dump($x);
    

## PHP Strings

A string is group of characters in a sentance. A string is writen with quotes either single or double.

### Manipulating PHP Strings ###
    
### Calculating the length of a string ###

To calculation the lenght of the string in number of characters you use the srtlen() function.

Examples

    echo strlen("Hello World!");   
    
    $x = "Hello World!";
    echo strlen($x);    // both outputs 
    
### Counting the words in a string ###

To get the word count in a string we use str_word_count().

Examples 

    echo str_word_count("Hello World!"); // outputs 2
    
### Replacing text in a string ###

To replace certain parts of a string with another you can use str_replace() to search the string for a value then replace that value. 

Syntax  str_replace( search-value(string), replacement(string), the-search-string(string) )

Examples 

    echo str_replace("world", "bob", "Hello world!"); // outputs Hello bob!
    
### Reversing a string ###

To reverse a string completely you can use the strrev() function.

Example

    echo strrev("Hello world!"); //outputs !dlrow olleH
    
## PHP Numbers ##

### Infinity ###

Infinity is a value given for a number that has exceeded the float max_size.

Examples 

    $x =1.9e411;
    var_dump($x); //outputs float(INF)
    
### NAN ###

NAN is the value that is given when a mathematical operation cannot be completed. 

    
