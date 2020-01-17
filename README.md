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
    var_dump($var)

### PHP Float

