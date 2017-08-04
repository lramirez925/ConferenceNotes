# An exercise in cleaner code - from legacy to maintainable
## By Gavin Pickin

1. What is clean code. 
    1. Clean Code by Robert C. Martin

1. Lowering cognitive Load
    1. Abstract complexity
        1. Shouldn't need to read 10 lines to know what it does. 
        1. Consitency. 

1. General rules of clean code. 
    1. Write code once but used many times. 
    1. Leave it cleaner than when you found it. (Boy Scout Rules)
    1. KISS - Keep it Simple Stupid
1. Naming, functions, comments
    1. Choose descriptive names. 
    1. Make names meaningful and distinct. 
    1. No magic numbers. Use Constants/ Enumerables. 
    1. Avoid encodings and prefixes to type information. 
        1. Possible conventino prefixes can be ok. 
            1. 
    1. No Acronyms. (Only Universal) 
    1. Examples
        1. Do
            1. customerAddress = getCustomerAddress()
            1. dangerColor = 'FF0000'
        1. Don't 
            1. redColor = 'FF0000' (colors can change in the app
    1. Use Conventions. 
        1. Constants all caps for example. 
    1. Short functions. (Easy to test)
        1. Many recomend 10-20 lines. 
            1. Exceptions occur.(Setting a lot of values into an object)
    1. Don't use to many arguments 
        1. Limit to 2 or 3
        1. Use a struct or object. 
        1. Ugh (not a fan due to signature being unknown)
    1. Flag arguments are a No NO
        1. Use multiple functions. 
    1. Use functions to hide complexity. 
    1. No side affects. (Always return a new object when editing values that are passed into arguments. )
    1. Comments 
        1. Comments should be at beginning of function. Don't comment end of function. 
        1. Try to let code speak for iteself where possible. 
        1. Comments should add value 
        1. Don't comment out code. 
        1. comment on the intent not how it works. 
        1. comment to explain consequences (side affects)
        1. ColdDoc or DocBox
            1. Can generate javadoc like documentation. 

1. Souce code, Formatting 
    1. Seperate code concepts. Vertically in your files. 
        1. Keep functions that are used together close to each other in the code. (Don't add a function to the bottom of the file when top function uses it. )
    1. Declare variables close to where they are needed. 
    1. Categorize folders. (Search, User, etc)
    1. Same conventions
    1. Look at the ortus solutions standards since coldfusion doesn't have one. https://github.com/Ortus-Solutions/coding-standards
    1. Keep lins short. 
    1. indent structs multi lines
    1. Don't format a file when you don't edit it. But format it if you do. Also commit 2 seperate commits. 1 for format and 1 for changed code. 
1. Lets look at some code. 