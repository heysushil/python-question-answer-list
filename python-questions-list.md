# Python Basic and Advance Questions list - be ready to solve them

## Agar question realted koi porblem hai to mujhe [YouTube Discussion](https://www.youtube.com/channel/UCphs2JfmIClR62wbyf76HDg/discussion) par puch sakte ho.

> Note: Sabhi questions searial wise hain, to kosis karo ki inhe isi serial me solve karo. Good luck

## String Questions:

1. Find all occurrences of “USA” in given string ignoring the case

    Expected Outcome:

    input_str = "Welcome to USA. usa awesome, isn't it?"

    The USA count is: 2

1. Given a string, return the sum and average of the digits that appear in the string, ignoring all other characters

    For Example: –

    sumAndAverage("English = 78 Science = 83 Math = 68 History = 65") = sum 294 Percentage is 73.5

        Output:

        Total Marks is: 294 Percentage is  73.5    

1. Given an input string, count occurrences of all characters within a string

    For Example:

    count("pynativepynvepynative") = {'p': 3, 'y': 3, 'n': 3, 'a': 2, 't': 2, 'i': 2, 'v': 3, 'e': 3}

        Output:

        {'p': 3, 'y': 3, 'n': 3, 'a': 2, 't': 2, 'i': 2, 'v': 3, 'e': 3}

## List questions:

1. Given a Python list you should be able to display Python list in the following order

        aLsit = [100, 200, 300, 400, 500]
        Expected output:

        [500, 400, 300, 200, 100]

1. Concatenate two lists index-wise

    list1 = ["M", "na", "i", "Ke"] 
    list2 = ["y", "me", "s", "lly"]

        Expected output:

        ['My', 'name', 'is', 'Kelly']

1. Given a Python list. Turn every item of a list into its square

    aList = [1, 2, 3, 4, 5, 6, 7]

        Expected output:

        [1, 4, 9, 16, 25, 36, 49]

1. Concatenate two lists in the following order

    list1 = ["Hello ", "take "]
    list2 = ["Dear", "Sir"]

        Expected output:

        ['Hello Dear', 'Hello Sir', 'take Dear', 'take Sir']

1. Given a two Python list. Iterate both lists simultaneously such that list1 should display item in original order and list2 in reverse order

    list1 = [10, 20, 30, 40]
    list2 = [100, 200, 300, 400]

        Expected output:

        10 400
        20 300
        30 200
        40 100

1. Remove empty strings from the list of strings

    list1 = ["Mike", "", "Emma", "Kelly", "", "Brad"]

        Expected output:

        ["Mike", "Emma", "Kelly", "Brad"]

1. Add item 7000 after 6000 in the following Python List

    list1 = [10, 20, [300, 400, [5000, 6000], 500], 30, 40]

        Expected output:

        [10, 20, [300, 400, [5000, 6000, 7000], 500], 30, 40]

1. Given a nested list extend it with adding sub list ["h", "i", "j"] in a such a way that it will look like the following list
Given List:

    list1 = ["a", "b", ["c", ["d", "e", ["f", "g"], "k"], "l"], "m", "n"]
    Sub List to be added = ["h", "i", "j"]

        Expected output:

        ['a', 'b', ['c', ['d', 'e', ['f', 'g', 'h', 'i', 'j'], 'k'], 'l'], 'm', 'n']

1. Given a Python list, find value 20 in the list, and if it is present, replace it with 200. Only update the first occurrence of a value

    list1 = [5, 10, 15, 20, 25, 50, 20]

        Expected output:

        list1 = [5, 10, 15, 200, 25, 50, 20]

1. Given a Python list, remove all occurrence of 20 from the list

    list1 = [5, 20, 15, 20, 25, 50, 20]

        Expected output:

        [5, 15, 25, 50]


## Python Tuple Exercise

1. Reverse the following tuple
    
    aTuple = (10, 20, 30, 40, 50)

        Expected output:

        (50, 40, 30, 20, 10)

1. Access value 20 from the following tuple
    
    aTuple = ("Orange", [10, 20, 30], (5, 15, 25))

        Expected output:

        20

1. Create a tuple with single item 50

1. Unpack the following tuple into 4 variables
    
    aTuple = (10, 20, 30, 40)

        Expected output:

        aTuple = (10, 20, 30, 40)
        # Your code
        print(a) # should print 10
        print(b) # should print 20
        print(c) # should print 30
        print(d) # should print 40

1. Swap the following two tuples

    tuple1 = (11, 22)
    tuple2 = (99, 88)

        Expected output:

        tuple1 = (99, 88)
        tuple2 = (11, 22)

1. Copy element 44 and 55 from the following tuple into a new tuple
    
    tuple1 = (11, 22, 33, 44, 55, 66)

        Expected output:

        tuple2 = (44, 55)

1. Modify the first item (22) of a list inside a following tuple to 222
    
    tuple1 = (11, [22, 33], 44, 55)

        Expected output:

        tuple1 = (11, [222, 33], 44, 55)

1. Sort a tuple of tuples by 2nd item
    
    tuple1 = (('a', 23),('b', 37),('c', 11), ('d',29))

        Expected output:

        (('c', 11), ('a', 23), ('d', 29), ('b', 37))

1. Counts the number of occurrences of item 50 from a tuple
    
    tuple1 = (50, 10, 60, 70, 50)

        Expected output:

        2

1. Check if all items in the following tuple are the same
    
    tuple1 = (45, 45, 45, 45)

        Expected output:

        True

## Dictinary related questions:

1. Diye gaye dict me brad ki salary update karke 8500 karni hai:

    sampleDict = {
        'emp1': {'name': 'Jhon', 'salary': 7500},
        'emp2': {'name': 'Emma', 'salary': 8000},
        'emp3': {'name': 'Brad', 'salary': 6500}
    }

        Expected output:
        sampleDict = {
            'emp1': {'name': 'Jhon', 'salary': 7500},
            'emp2': {'name': 'Emma', 'salary': 8000},
            'emp3': {'name': 'Brad', 'salary': 8500}
        }

1. Ye do list hai inko dictionary me convert karna hai:

    keys = ['Ten', 'Twenty', 'Thirty']
    values = [10, 20, 30]
        
        Output kuch aysa hona chaiye: 
        {'Ten': 10, 'Twenty': 20, 'Thirty': 30}

1. In 2 dictionary ko ek sath marg karo:

    dict1 = {'Ten': 10, 'Twenty': 20, 'Thirty': 30}
    dict2 = {'Thirty': 30, 'Fourty': 40, 'Fifty': 50}

        Aur iska output kuch aysa mulna cahiye:
        {'Ten': 10, 'Twenty': 20, 'Thirty': 30, 'Fourty': 40, 'Fifty': 50}

1. Is diye gaye dict mese history ki value ko show karao:

    sampleDict = { 
    "class":{ 
        "student":{ 
            "name":"Mike",
            "marks":{ 
                "physics":70,
                "history":80
            }
        }
    }
    }

        Expected answer: 80

1. Diyegaye list ko as a key aur diyegaye dict ko as a value set karo:

    employees = ['Kelly', 'Emma', 'John']
    defaults = {"designation": 'Application Developer', "salary": 8000}

1. Dict me check karna hai ki kya 200 value exist karta hai ya nahi:
    
    sampleDict = {'a': 100, 'b': 200, 'c': 300}

        Expected output:
        True

1. Diye gaye dict me city ko rename karke location karna hai:

    sampleDict = {
    "name": "Kelly",
    "age":25,
    "salary": 8000,
    "city": "New york"
    }
 
        Expected output:
        {
        "name": "Kelly",
        "age":25,
        "salary": 8000,
        "location": "New york"
        }

1. Diye gaye dict me jis subject ka bhi marks sabse kam hai usko find kar ke show karna hai:

    sampleDict = {
    'Physics': 82,
    'Math': 65,
    'history': 75
    }

        Expected output:
        Math


## Set questions:

1. Set me diye gaye list ko add karna hai:

    sampleSet = {"Yellow", "Orange", "Black"}
    sampleList = ["Blue", "Green", "Red"]

        Expected output:
        In set item order is not a concern
        {'Green', 'Yellow', 'Black', 'Orange', 'Red', 'Blue'}

1. 2no set me se identical item ko find karna hai:

    set1 = [10, 20, 30, 40, 50]
    set2 = [30, 40, 50, 60, 70]

        Expected output:

        {40, 50, 30}

1. 2no set mese unique items ko find karan hai:

    set1 = {10, 20, 30, 40, 50}
    set2 = {30, 40, 50, 60, 70}

        Expected output:
        {70, 40, 10, 50, 20, 60, 30}

1. 2no set me se 1st set me jobhi item unique hai kewal unko dikhana hai:

    set1 = {10, 20, 30}
    set2 = {20, 40, 50}

        Expected output:
        set1 = {10, 30}

1. Diye gaye set mese 10,20,30 ek baar me hi remove karne hai:

	set1 = {10, 20, 30, 40, 50}

        Expected output:
        {40, 50}

1. Diye gaye set me jo bhi number dono set me common na ho unko dikhana hai:
	
    set1 = {10, 20, 30, 40, 50}
    set2 = {30, 40, 50, 60, 70}

        Expected output:
        {20, 70, 10, 60}

1. Set 1 mese wo values ko remove karna hai jo set 2 me nahi hai:
	
    set1 = {10, 20, 30, 40, 50}
    set2 = {30, 40, 50, 60, 70}

        Expected output:
        {40, 50, 30}

1. 2no set me jobhi common values hai wo show karna hai:

    set1 = {10, 20, 30, 40, 50}
    set2 = {60, 70, 80, 90, 10}

        Expected output:
        Two sets have items in common
        {10}


## Python Input and Output Exercise with File Handling 

1. Accept two numbers from the user and calculate multiplication

1. Display “My Name Is James” as “My**Name**Is**James” using output formatting of a print() function

    Expected Output:

    Use print() statement formatting to display ** separator between each word.

    For example: print('My', 'Name', 'Is', 'James') will display MyNameIsJames

    So use one of the formatting argument of print() to turn the output into My**Name**Is**James

1. Convert decimal number to octal using print() output formatting

        Expected Output:

        Display decimal number 8 as 10

1.  Display float number with 2 decimal places using print()

        Expected Output:

        Display 458.541315 as 458.54        

1. Accept list of 5 float numbers as a input from user

        Expected Output:

        Numbers can be any

        [78.6, 78.6, 85.3, 1.2, 3.5]

1.  write all file content into new file by skiping line 5 from following file

        test.txt file:

        line1
        line2
        line3
        line4
        line5
        line6
        line7

        newFile.txt should be

        line1
        line2
        line3
        line4
        line6
        line7

1. Accept any three string from one input() call

1. You have the following data.

        totalMoney = 1000
        quantity = 3
        price = 450

    display above data using string.format() method

        I have 1000 dollars so I can buy 3 football for 450.00 dollars.

1. How to check file is empty or not

1. Read line number 4 from the following file

                test.txt file:

                line1
                line2
                line3
                line4
                line5
                line6
                line7

## function questions:

1. Given a string of odd length greater 7, return a string made of the middle three chars of a given String.

    For example: –

    getMiddleThreeChars("JhonDipPeta") → "Dip"
    getMiddleThreeChars("Jasonay") → "son"

        Expected Output:

        Original String is JhonDipPeta
        Middle three chars are Dip
        Original String is Jasonay
        Middle three chars are son

1. Given 2 strings, s1 and s2, create a new string by appending s2 in the middle of s1

    Expected Outcome:

    appendMiddle("Chrisdem", IamNewString) → "ChrIamNewStringisdem"

        Output:

        Original Strings are Chrisdem IamNewString
        After appending new string in middle ChrIamNewStringisdem    

1. arrange String characters such that lowercase letters should come first
Given input String of combination of the lower and upper case arrange characters in such a way that all lowercase letters should come first.

    Expected Output:

    input_String = PyNaTive

    arranging characters giving precedence to lowercase letters:
    yaivePNT

1. Count all lower case, upper case, digits, and special symbols from a given string

        Expected Outcome:

        input_str = "P@#yn26at^&i5ve"

        Total counts of chars, digits,and symbols 
        Chars = 8 
        Digits = 3 
        Symbol = 4

1.  Given two strings, s1 and s2, create a mixed String
Note: create a third-string made of the first char of s1 then the last char of s2, Next, the second char of s1 and second last char of s2, and so on. Any leftover chars go at the end of the result.

    Expected Outcome:

    Sponsored by Advertising Partner
    Sponsored Video
    Watch to learn more
    SEE MORE
    mixString("Abc", "Xyz") = AzbycX

1. String characters balance Test
We’ll say that a String s1 and s2 is balanced if all the chars in the string1 are there in s2. characters position doesn’t matter.

    For Example: –

    stringBalanceCheck(yn, Pynative) = True

        Output:

        s1 and s2 are balanced True
        s1 and s2 are balanced False

1.         