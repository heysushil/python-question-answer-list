# Python Basic and Advance Questions list - be ready to solve them

## Agar question realted koi porblem hai to mujhe [YouTube Discussion](https://www.youtube.com/channel/UCphs2JfmIClR62wbyf76HDg/discussion) par puch sakte ho.

> Note: Sabhi questions searial wise hain, to kosis karo ki inhe isi serial me solve karo. Good luck

> Note: Sabhi answer usi sequence me hain jinme questions hai

## List questions:



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
        