# Python Basic and Advance Questions list - be ready to solve them

## Agar question realted koi porblem hai to mujhe [YouTube Discussion](https://www.youtube.com/channel/UCphs2JfmIClR62wbyf76HDg/discussion) par puch sakte ho.

> Note: Sabhi questions searial wise hain, to kosis karo ki inhe isi serial me solve karo. Good luck

> Note: Sabhi answer usi sequence me hain jinme questions hai

## String Questions:

1. Find all occurrences of “USA” in given string ignoring the case

                inputString = "Welcome to USA. usa awesome, isn't it?"
                substring = "USA"
                tempString = inputString.lower()
                count = tempString.count(substring.lower())
                print("The USA count is:", count)

1. Given a string, return the sum and average of the digits that appear in the string, ignoring all other characters

                import re

                inputStr = "English = 78 Science = 83 Math = 68 History = 65"
                markList = [int(num) for num in re.findall(r'\b\d+\b', inputStr)]
                totalMarks = 0
                for mark in markList:
                  totalMarks+=mark

                percentage = totalMarks/len(markList)  
                print("Total Marks is:", totalMarks, "Percentage is ", percentage)

1. Given an input string, count occurrences of all characters within a string

                inputStr = "pynativepynvepynative"
                countDict = dict()
                for char in inputStr:
                  count = inputStr.count(char)
                  countDict[char]=count
                print(countDict)


## List questions:

1. Given a Python list you should be able to display Python list in the following order

                aList = [100, 200, 300, 400, 500]
                aList = aList[::-1]
                print(aList)

1. Concatenate two lists index-wise

        Note: We need to use list comprehension and zip() function as follows

                list1 = ["M", "na", "i", "Ke"] 
                list2 = ["y", "me", "s", "lly"]
                list3 = [i + j for i, j in zip(list1, list2)]
                print(list3)

1. Given a Python list. Turn every item of a list into its square

                aList = [1, 2, 3, 4, 5, 6, 7]
                aList =  [x * x for x in aList]
                print(aList)

1. Concatenate two lists in the following order

                list1 = ["Hello ", "take "]
                list2 = ["Dear", "Sir"]

                resList = [x+y for x in list1 for y in list2]
                print(resList)

1. Given a two Python list. Iterate both lists simultaneously such that list1 should display item in original order and list2 in reverse order

                list1 = [10, 20, 30, 40]
                list2 = [100, 200, 300, 400]

                for x, y in zip(list1, list2[::-1]):
                print(x, y)

1. Remove empty strings from the list of strings

        Note: We can use a filter() function to remove None type from the list


                list1 = ["Mike", "", "Emma", "Kelly", "", "Brad"]
                resList = list(filter(None, list1))
                print(resList)

1. Add item 7000 after 6000 in the following Python List

        Note: Use the append() method

                list1 = [10, 20, [300, 400, [5000, 6000], 500], 30, 40]
                list1[2][2].append(7000)
                print(list1)        

1. Given a nested list extend it with adding sub list ["h", "i", "j"] in a such a way that it will look like the following list
Given List:

                list1 = ["a", "b", ["c", ["d", "e", ["f", "g"], "k"], "l"], "m", "n"]
                subList = ["h", "i", "j"]

                list1[2][1][2].extend(subList)
                print(list1)

1. Given a Python list, find value 20 in the list, and if it is present, replace it with 200. Only update the first occurrence of a value

                list1 = [5, 10, 15, 20, 25, 50, 20]

                index = list1.index(20)
                list1[index] = 200
                print(list1)

1. Given a Python list, remove all occurrence of 20 from the list

        Note: Use the list comprehension

                list1 = [5, 20, 15, 20, 25, 50, 20]

                def removeValue(sampleList, val):
                return [value for value in sampleList if value != val]
                resList = removeValue(list1, 20)
                print(resList)        

## Python Tuple Exercise

1. Reverse the following tuple

                aTuple = (10, 20, 30, 40, 50)
                aTuple = aTuple[::-1]
                print(aTuple)

1. Access value 20 from the following tuple

                aTuple = ("Orange", [10, 20, 30], (5, 15, 25))
                print(aTuple[1][1])

1. Create a tuple with single item 50

                aTuple = (50, )
                print(aTuple)

        Note: If you want to create a single value tuple, you must indicate it by adding a comma just before the closing parentheses.

1. Unpack the following tuple into 4 variables

                aTuple = (10, 20, 30, 40)
                a, b, c, d = aTuple
                print(a)
                print(b)
                print(c)
                print(d)

1. Swap the following two tuples

                tuple1 = (11, 22)
                tuple2 = (99, 88)
                tuple1, tuple2 = tuple2, tuple1
                print(tuple2)
                print(tuple1)

1. Copy element 44 and 55 from the following tuple into a new tuple

                tuple1 = (11, 22, 33, 44, 55, 66)
                tuple2 = tuple1[3:-1]
                print(tuple2)

1. Modify the first item (22) of a list inside a following tuple to 222

                tuple1 = (11, [22, 33], 44, 55)
                tuple1[1][0] = 222
                print(tuple1)

1. Sort a tuple of tuples by 2nd item

                tuple1 = (('a', 23),('b', 37),('c', 11), ('d',29))
                tuple1 = tuple(sorted(list(tuple1), key=lambda x: x[1]))
                print(tuple1)

1. Counts the number of occurrences of item 50 from a tuple

                tuple1 = (50, 10, 60, 70, 50)
                print(tuple1.count(50))

1. Check if all items in the following tuple are the same

                def check(sampleTuple):
                return all(i == sampleTuple[0] for i in sampleTuple)

                tuple1 = (45, 45, 45, 45)
                print(check(tuple1))

## Dictionary related answers

1. Diye gaye dict me brad ki salary update karke 8500 karni hai:

        sampleDict['emp3']['salary'] = 8500
        print(sampleDict)<

1. Ye do list hai inko dictionary me convert karna hai: 

        keys = ['Ten', 'Twenty', 'Thirty']
        values = [10, 20, 30]

        sampleDict = dict(zip(keys, values))
        print(sampleDict)

1. In 2 dictionary ko ek sath marg karo:

    dict1 = {'Ten': 10, 'Twenty': 20, 'Thirty': 30}
    dict2 = {'Thirty': 30, 'Fourty': 40, 'Fifty': 50}

        dict3 = dict1.copy()
        dict3.update(dict2)
        print(dict3)

1. Is diye gaye dict mese history ki value ko show karao:

        print(sampleDict['class']['student']['marks']['history'])

1. Diyegaye list ko as a key aur diyegaye dict ko as a value set karo:

        employees = ['Kelly', 'Emma', 'John']
        defaults = {"designation": 'Application Developer', "salary": 8000}

        resDict = dict.fromkeys(employees, defaults)
        print(resDict)

        # Individual data
        print(resDict["Kelly"])

1. Dict me check karna hai ki kya 200 value exist karta hai ya nahi:
	
        sampleDict = {'a': 100, 'b': 200, 'c': 300}
        print(200 in sampleDict.values())

1. Diye gaye dict me city ko rename karke location karna hai:

        sampleDict = {
        "name": "Kelly",
        "age":25,
        "salary": 8000,
        "city": "New york"
        }
        
        sampleDict['location'] = sampleDict.pop('city')
        print(sampleDict)

1. Diye gaye dict me jis subject ka bhi marks sabse kam hai usko find kar ke show karna hai:

        sampleDict = {
        'Physics': 82,
        'Math': 65,
        'history': 75
        }
        print(min(sampleDict, key=sampleDict.get))

1. Diye gaye dict mese niche bataye keys ka use kar ke new dict banao:

        sampleDict = { 
        "name": "Kelly",
        "age":25, 
        "salary": 8000, 
        "city": "New york" }

        keys = ["name", "salary"]

        newDict = {k: sampleDict[k] for k in keys}
        print(newDict)

1. Dict mese following keys ko remove karna hai:

        sampleDict = {
        "name": "Kelly",
        "age":25,
        "salary": 8000,
        "city": "New york"
        }
        keysToRemove = ["name", "salary"]

        sampleDict = {k: sampleDict[k] for k in sampleDict.keys() - keysToRemove}
        print(sampleDict)


# Set answers:

1. Set me diye gaye list ko add karna hai:

        sampleSet = {"Yellow", "Orange", "Black"}
        sampleList = ["Blue", "Green", "Red"]
        sampleSet.update(sampleList)
        print(sampleSet)

1. 2no set me se identical item ko find karna hai:

        set1 = {10, 20, 30, 40, 50}
        set2 = {30, 40, 50, 60, 70}

        print(set1.intersection(set2))

1. 2no set mese unique items ko find karan hai:

        set1 = {10, 20, 30, 40, 50}
        set2 = {30, 40, 50, 60, 70}

        print(set1.union(set2))

1. 2no set me se 1st set me jobhi item unique hai kewal unko dikhana hai:
	
        set1 = {10, 20, 30}
        set2 = {20, 40, 50}

        set1.difference_update(set2)
        print(set1)

1. Diye gaye set mese 10,20,30 ek baar me hi remove karne hai:

        set1 = {10, 20, 30, 40, 50}
        set1.difference_update({10, 20, 30})
        print(set1)

1. Diye gaye set me jo bhi number dono set me common na ho unko dikhana hai:

        set1 = {10, 20, 30, 40, 50}
        set2 = {30, 40, 50, 60, 70}

        print(set1.symmetric_difference(set2))

1. Set 1 mese wo values ko remove karna hai jo set 2 me nahi hai:

        set1 = {10, 20, 30, 40, 50}
        set2 = {30, 40, 50, 60, 70}

        set1.intersection_update(set2)
        print(set1)

1. 2no set me jobhi common values hai wo show karna hai:

        set1 = {10, 20, 30, 40, 50}
        set2 = {60, 70, 80, 90, 10}

        if set1.isdisjoint(set2):
        print("Two sets have no items in common")
        else:
        print("Two sets have items in common")
        print(set1.intersection(set2))


## Python Input and Output Exercise with File Handling 

1. Accept two numbers from the user and calculate multiplication

                num1 = int(input("Enter first number "))
                num2 = int(input("Enter second number "))

                print("\n")
                res = num1 + num2
                print("Sum is", res)

1. Display “My Name Is James” as “My**Name**Is**James” using output formatting of a print() function

                print('My', 'Name', 'Is', 'James', sep='**')

1. Convert decimal number to octal using print() output formatting

                print('%o,' % (8))

1.  Display float number with 2 decimal places using print()

                print('%.2f' % 458.541315)

1. Accept list of 5 float numbers as a input from user

                floatNumbers = []
                n = int(input("Enter the list size : "))

                print("\n")
                for i in range(0, n):
                print("Enter number at location", i, ":")
                item = float(input())
                floatNumbers.append(item)
                
                print("User List is ", floatNumbers)

1.  write all file content into new file by skiping line 5 from following file

                count = 0
                with open("test.txt", "r") as fp:
                lines = fp.readlines()
                count = len(lines)
                with open("newFile.txt", "w") as fp:
                for line in lines:
                        if (count == 3):
                        count -= 1
                        continue
                        else:
                        fp.write(line)
                        count-=1

1. Accept any three string from one input() call

                str1, str2, str3 = input("Enter three string").split()
                print(str1, str2, str3)

                Output:

                Enter three string jhon emma, kelly
                jhon emma, kelly                

1. You have the following data.

                quantity = 3
                totalMoney = 1000
                price = 450
                statement1 = "I have {1} dollars so I can buy {0} football for {2:.2f} dollars."
                print(statement1.format(quantity, totalMoney, price))

1. How to check file is empty or not

                import os
                print(os.stat("test.txt").st_size == 0)        

1. Read line number 4 from the following file

                with open("test.txt", "r") as fp:
                lines = fp.readlines()
                print(lines[3])
        
## Function answers:

1. Given a string of odd length greater 7, return a string made of the middle three chars of a given String

                def getMiddleThreeChars(sampleStr):
                        middleIndex = int(len(sampleStr) /2)
                        print("Original String is", sampleStr)
                        middleThree = sampleStr[middleIndex-1:middleIndex+2]
                        print("Middle three chars are", middleThree)
                
                getMiddleThreeChars("JhonDipPeta")
                getMiddleThreeChars("Jasonay")                

1. Given 2 strings, s1 and s2, create a new string by appending s2 in the middle of s1

                def appendMiddle(s1, s2):
                        middleIndex = int(len(s1) /2)
                        print("Original Strings are", s1, s2)
                        middleThree = s1[:middleIndex-1:]+ s2 +s1[middleIndex-1:]
                        print("After appending new string in middle", middleThree)
                
                appendMiddle("Chrisdem", "IamNewString")

1. arrange String characters such that lowercase letters should come first
Given input String of combination of the lower and upper case arrange characters in such a way that all lowercase letters should come first.

                inputStr = "PyNaTive"
                words = inputStr.split()
                lower = []
                upper = []
                for char in inputStr:
                        if char.islower():
                                lower.append(char)
                        else:
                                upper.append(char)
                sortedString = ''.join(lower + upper)
                print("\n arranging characters giving precedence to lowercase letters:")
                print(sortedString)

1. Count all lower case, upper case, digits, and special symbols from a given string

                def findDigitsCharsSymbols(inputString):
                        words = inputString.split()
                        charCount = 0
                        digitCount = 0
                        symbolCount = 0
                        for char in inputString:
                                if char.islower() or char.isupper():
                                        charCount+=1
                                elif char.isnumeric():
                                        digitCount+=1
                                else:
                                        symbolCount+=1
                        
                        print("Chars = ", charCount, "Digits = ", digitCount, "Symbol = ", symbolCount)
                
                inputString = "P@#yn26at^&i5ve"
                print("total counts of chars, digits,and symbols \n")

                findDigitsCharsSymbols(inputString)

1.  Given two strings, s1 and s2, create a mixed String
Note: create a third-string made of the first char of s1 then the last char of s2, Next, the second char of s1 and second last char of s2, and so on. Any leftover chars go at the end of the result.

                def mixString(s1, s2):
                  s2 = s2[::-1]
                  lengthS1 = len(s1)
                  lengthS2 = len(s2)
                  length  = lengthS1 if lengthS1 > lengthS2 else lengthS2 
                  resultString=""
                  for i in range(length):
                    if(i < lengthS1):
                      resultString = resultString + s1[i]
                    if(i < lengthS2):
                      resultString = resultString + s2[i]

                  print(resultString)

                s1 = "Abc"
                s2 = "Xyz"
                mixString(s1, s2)

1. String characters balance Test
We’ll say that a String s1 and s2 is balanced if all the chars in the string1 are there in s2. characters position doesn’t matter.

                def stringBalanceCheck(s1, s2):
                  flag = True
                  for char in s1:
                    if char in s2:
                      continue
                    else:
                      flag = False
                  return flag

                s1 = "yn"
                s2 = "Pynative"
                flag = stringBalanceCheck(s1, s2)
                print("s1 and s2 are balanced", flag)

                s1 = "ynf"
                s2 = "Pynative"
                flag = stringBalanceCheck(s1, s2)
                print("s1 and s2 are balanced", flag)

