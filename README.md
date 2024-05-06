
{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "d009ce83",
   "metadata": {},
   "source": [
    "# BASIC PYTHON PROJECT"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "ae3eb113",
   "metadata": {},
   "source": [
    "# what is Python?\n",
    "Python is a high-level, interpreted programming language known for its simplicity and readability. \n",
    "Created by Guido van Rossum and first released in 1991, Python has gained immense popularity due to its versatility and ease of use. \n",
    "It supports multiple programming paradigms, including procedural, object-oriented, and functional programming."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "b516581b",
   "metadata": {},
   "source": [
    "IF :\n",
    "In Python, if and else are control flow statements used for decision making within a program. They allow you to execute certain blocks of code based on whether a given condition is true or false.\n",
    "    \n",
    "    "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "34d9039d",
   "metadata": {},
   "source": [
    "ELSE: In Python,the condition is false in if statement ,the block of code under else will be executed "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "1d66bb4d",
   "metadata": {},
   "source": [
    "NESTED IF:\n",
    "Nested if statements are conditional statements within other conditional statements (usually within the if or else block of another if or else statement). They allow for more complex decision-making logic by providing multiple levels of conditions to be evaluated."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "aec8123c",
   "metadata": {},
   "source": [
    "# THE EXAMPLE ON IF,ELSE,NESTED IF:"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "0f167fa0",
   "metadata": {},
   "source": [
    "# Question 1: to check the given number is greater than 5 or not"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 1,
   "id": "5282f4b1",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "x is greater than 5\n"
     ]
    }
   ],
   "source": [
    "\n",
    "x = 10\n",
    "\n",
    "if x > 5:\n",
    "    print(\"x is greater than 5\")\n",
    "else:\n",
    "    print(\"x is not greater than 5\")"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "b9be23cd",
   "metadata": {},
   "source": [
    "# Question 2: To check which grade we got given by the user"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "id": "aab54e09",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter the marks85\n",
      "B\n"
     ]
    }
   ],
   "source": [
    "# Question 2:\n",
    "grade = int(input(\"Enter the marks\"))\n",
    "\n",
    "if grade >= 90:\n",
    "    print(\"A\")\n",
    "elif grade >= 80:\n",
    "    print(\"B\")\n",
    "elif grade >= 70:\n",
    "    print(\"C\")\n",
    "elif grade >= 60:\n",
    "    print(\"D\")\n",
    "else:\n",
    "    print(\"F\")\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "f4c56346",
   "metadata": {},
   "source": [
    "# Question 3:To check the where it is need to take the umbrella  using boolean values"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 7,
   "id": "c30faae4",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "No need for an umbrella today.\n"
     ]
    }
   ],
   "source": [
    "is_raining = False\n",
    "\n",
    "if is_raining:\n",
    "    print(\"Remember to take an umbrella.\")\n",
    "else:\n",
    "    print(\"No need for an umbrella today.\")\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "f747f1fa",
   "metadata": {},
   "source": [
    "# Question 4: To check the which given numbers are  "
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "id": "c90299eb",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "x is greater than 5\n",
      "y is greater than 3\n"
     ]
    }
   ],
   "source": [
    "# QUSETION 4\n",
    "x = 10\n",
    "y = 5\n",
    "\n",
    "if x > 5:\n",
    "    print(\"x is greater than 5\")\n",
    "    if y > 3:\n",
    "        print(\"y is greater than 3\")\n",
    "    else:\n",
    "        print(\"y is not greater than 3\")\n",
    "else:\n",
    "    print(\"x is not greater than 5\")\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "d0d4f93a",
   "metadata": {},
   "source": [
    "# FOR LOOP IN PYTHON:\n",
    "    In Python, the for loop is used to iterate over a sequence (such as a list, tuple, string, or range) or any other iterable object. It executes a block of code repeatedly for each item in the sequence."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "88b14961",
   "metadata": {},
   "source": [
    "#  Question 5: Write a program to dislplay product of the digts of a number accepted from this user"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "id": "b5e9461a",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "enter num:2344\n",
      "96\n"
     ]
    }
   ],
   "source": [
    "num=int(input(\"enter num:\"))\n",
    "p=1\n",
    "for i in range(1,num):\n",
    "    if num>0:\n",
    "        i=num%10\n",
    "        p=p*i\n",
    "        num=num//10\n",
    "print(p)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a85cd0eb",
   "metadata": {},
   "source": [
    "# Question 6: how many prime numbers and composite numbers are there from 1 to  100"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 8,
   "id": "f52a278f",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "the number of prime number from 1 to 100 0\n",
      "the number of prime number from 1 to 100 1\n"
     ]
    }
   ],
   "source": [
    "#prime\n",
    "#2-1,2\n",
    "#2-1,3\n",
    "#29-1,29\n",
    "#composite\n",
    "#4-1,24\n",
    "#25-1,5,25\n",
    "#10-1,2,5,10\n",
    "\n",
    "for i in range(2,101):\n",
    "    c=0\n",
    "    c_prime=0\n",
    "    c_comp=0\n",
    "    for j in range(1,i+1):\n",
    "        if i % j == 0:\n",
    "            c=c+1\n",
    "    if c==2 :   \n",
    "        c_prime= c_prime +  1\n",
    "    else:    \n",
    "        c_comp=c_comp + 1\n",
    "\n",
    "print(\"the number of prime number from 1 to 100\",c_prime)\n",
    "print(\"the number of prime number from 1 to 100\",c_comp)        "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "9d80017f",
   "metadata": {},
   "source": [
    "# Question 7: Write a program to get the factorial of any user defined input"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 9,
   "id": "9a589a39",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter the value:4\n",
      "24\n"
     ]
    }
   ],
   "source": [
    "#get the factorial of any user defined input\n",
    "\n",
    "n=int(input(\"Enter the value:\"))\n",
    "factorial=1\n",
    "for i in range(1,n+1):\n",
    "    factorial=factorial*i\n",
    "print(factorial)    \n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "5350f2f6",
   "metadata": {},
   "source": [
    "#  Question 8:Write a program to get the sum of all even numbers from 1 to 50"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "id": "dd07678e",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "enter the num:10\n",
      "the sum of all even number 1 to 50 is: 240\n"
     ]
    }
   ],
   "source": [
    "#get the sum of all even numbers from 1 to 50\n",
    "num=int(input(\"enter the num:\"))\n",
    "s=0\n",
    "for i in range (1,50):\n",
    "    if i%2==0:\n",
    "        s=s+num\n",
    "\n",
    "print(\"the sum of all even number 1 to 50 is:\",s)        "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "42e9b0e1",
   "metadata": {},
   "source": [
    "# WHILE LOOP IN PYTHON:\n",
    "In Python, the while loop is another type of loop that repeatedly executes a block of code as long as a specified condition is true. It continues looping until the condition becomes false. This is useful when you don't know in advance how many times the loop will need to execute."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "5e2f58d8",
   "metadata": {},
   "source": [
    "# Question 9: Write a Program display only numeric values from the list using while loop"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 11,
   "id": "bb4d721d",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "23\n",
      "24\n",
      "25\n"
     ]
    }
   ],
   "source": [
    "n=[\"Gaya\",23,\"Yashwanth\",24,\"Vijay\",25]\n",
    "i=0\n",
    "while i<len(n):\n",
    "    if isinstance(n[i],int):\n",
    "        print(n[i])\n",
    "    i=i+1"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a51ff1a4",
   "metadata": {},
   "source": [
    "# Question 10: Write a program to take a list of random number os your choices and get only the prime number from list"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 9,
   "id": "dc291448",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "1 23\n",
      "3 52\n",
      "5 26\n",
      "7 32\n"
     ]
    }
   ],
   "source": [
    "mylist = [11,23,44,52,4,26,27,32]\n",
    "i=0\n",
    "while i<len(mylist):\n",
    "    if i%2!=0:\n",
    "        print(i,mylist[i])\n",
    "    i=i+1 \n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "e0184ad5",
   "metadata": {},
   "source": [
    "#  Question 11:Write a program get only names from the list using break statement in the loop\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 14,
   "id": "be6c785b",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Satya\n",
      "Pavs\n",
      "Bilal\n",
      "Yash\n",
      "himan\n"
     ]
    }
   ],
   "source": [
    "i=0\n",
    "li=[\"Satya\",\"Pavs\",\"Bilal\",\"Yash\",\"himan\",2,32,283,20,387,28,19]\n",
    "\n",
    "while i<len(li):\n",
    "    if type(li[i])==int:\n",
    "        break\n",
    "    print(li[i])\n",
    "    i=i+1     \n",
    "    \n",
    "    "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "16b34de8",
   "metadata": {},
   "source": [
    "# DATA STRUCTURE IN PYTHON\n",
    "1:TUPLE\n",
    "2:LIST\n",
    "3:DICTIONARY\n",
    "4:SET    "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "bcdd3200",
   "metadata": {},
   "source": [
    "# TUPLE:In Python, a tuple is an immutable sequence data type. It is similar to a list but with the key difference that tuples cannot be changed once they are created. Tuples are defined by enclosing comma-separated values within parentheses ()."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "dcc5565e",
   "metadata": {},
   "source": [
    "EXAMPLE ON TUPLE:"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "cccc6f03",
   "metadata": {},
   "source": [
    "#  Question 12:how to create a tuple"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 17,
   "id": "42fc10a9",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "(1, 2, 3, 4, 5)\n"
     ]
    }
   ],
   "source": [
    "my_tuple = (1, 2, 3, 4, 5)\n",
    "print(my_tuple)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a02a8ad1",
   "metadata": {},
   "source": [
    "# Question 13:how to add two tuple"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 20,
   "id": "a1561420",
   "metadata": {},
   "outputs": [],
   "source": [
    "tuple1=(1,2,3)\n",
    "tuple2=(4,5,6)\n",
    "result=tuple1+tuple2  #Union\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "ac43730d",
   "metadata": {},
   "source": [
    "# LIST:\n",
    "    In Python, a list is a versatile and mutable data structure that can contain elements of different data types. Lists are ordered collections, meaning the elements maintain their position and can be accessed via indices. Lists are defined by enclosing comma-separated values within square brackets []."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "9f7be886",
   "metadata": {},
   "source": [
    "# EXAMPLE ON LIST:"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a453e99b",
   "metadata": {},
   "source": [
    "# Question 14: How to create a list"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 22,
   "id": "837ee365",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "['Dhivya', 'Himanshu', 'Pavithra', 'Bilal', 'Jaspreet', 'VijayKumar']"
      ]
     },
     "execution_count": 22,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "s_list=[\"Dhivya\",\"Himanshu\",\"Pavithra\",\"Bilal\",\"Jaspreet\",\"VijayKumar\"]\n",
    "s_list"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "6c166104",
   "metadata": {},
   "source": [
    "# Question 15: how to append the the name in a new list which are present ata even indexes"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "id": "11c848bc",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "['Himanshu', 'Vijay', 'Sidhant', 'Dhivya', 'Bilal', 'Yash', 'Shiny', 'Jaspreet', 'Rasika', 'Satyajit']\n"
     ]
    }
   ],
   "source": [
    "names = ['Himanshu','Swagath','Vijay','Gaya',\"Sidhant\",'Pavithra','Dhivya','Chetan','Bilal','Yashwanth','Yash','Jyothi','Shiny','Kajol','Jaspreet','Shankar','Rasika','Akash','Satyajit']\n",
    "new=[]\n",
    "\n",
    "for i in range(len(names)):\n",
    "    if i%2==0:\n",
    "        new.append(names[i]) #inedexing  on values done here \n",
    "print(new)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a07e2d2e",
   "metadata": {},
   "source": [
    "#  Question 16:How to append the names in a new list  whose are starting with 'S'\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 31,
   "id": "28a6a619",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "['Swagath', 'Sidhant', 'Shiny', 'Shankar', 'Satyajit']\n"
     ]
    }
   ],
   "source": [
    "#running the loop on the values\n",
    "new1=[]\n",
    "for i in names:\n",
    "    if i.startswith('S'):\n",
    "        new1.append(i)\n",
    "\n",
    "        \n",
    "print(new1)        "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "e9b48155",
   "metadata": {},
   "source": [
    "# Question 17:How to get the list by there index values"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 33,
   "id": "a1010064",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "0 90\n",
      "1 20\n",
      "2 30\n",
      "3 40\n",
      "4 50\n",
      "5 70\n",
      "6 90\n"
     ]
    }
   ],
   "source": [
    "my_list=[90,20,30,40,50,70,90]\n",
    "my_list\n",
    "for index,value in enumerate(my_list):\n",
    "    print(index,value)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "5427d6d0",
   "metadata": {},
   "source": [
    "# LIST COMPREHENSION:"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "d47957b0",
   "metadata": {},
   "source": [
    "#  Question 18:how do you get the lengths of each name in a new list"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 36,
   "id": "260ded2a",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[300, 600]"
      ]
     },
     "execution_count": 36,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "#you have to get the lengths of each name in a new list\n",
    "l=[10,20,30,40,50,60]\n",
    "o=[]\n",
    "o=[(i*10) for i in l if i%3==0]\n",
    "o"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "06439688",
   "metadata": {},
   "source": [
    "# Question 19: How do you get the len of values in the list?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 37,
   "id": "b4d841fb",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[8, 7, 5, 4, 7, 8, 6, 6, 5, 9, 4, 6, 5, 5, 8, 7, 6, 5, 8]"
      ]
     },
     "execution_count": 37,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "names = ['Himanshu','Swagath','Vijay','Gaya',\"Sidhant\",'Pavithra','Dhivya','Chetan','Bilal','Yashwanth','Yash','Jyothi','Shiny','Kajol','Jaspreet','Shankar','Rasika','Akash','Satyajit']\n",
    "output_lengths=[len(names[i]) for i in range(len(names)) ]\n",
    "output_lengths"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "00d2477d",
   "metadata": {},
   "source": [
    "#  Question 20 :How do you  get only odd num and add them in new in list after multiplyiing them with 1000"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 38,
   "id": "a1b38eb4",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[121000, 23000, 45000, 131000, 21000, 133000, 33000]"
      ]
     },
     "execution_count": 38,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "b=[14,102,121,23,130,26,34,45,148,131,128,21,118,133,144,33]\n",
    "\n",
    "b_new=[(i*1000) for i in b if i%2!=0]\n",
    "b_new\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "4b85ee36",
   "metadata": {},
   "source": [
    "# Question 21: you have to store their salaries in a new list after multiplying each value with 1000"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 7,
   "id": "2b32be07",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[23500.0, 24000, 6000, 31200.0, 32400.0, 25600.0, 34500.0, 31500.0, 40600.0, 41500.0, 36500.0]\n"
     ]
    }
   ],
   "source": [
    "emp = [101,23.5,102,24,6,103,31.2,104,32.4,105,25.6,106,34.5,107,31.5,108,40.6,109,41.5,110,36.5]\n",
    "#in  the emp list  ten employess id and their salaries are given\n",
    "\n",
    "\n",
    "new=[]\n",
    "new=[(i*1000) for i in emp if i<100]\n",
    "print(new)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "43602fa6",
   "metadata": {},
   "source": [
    "# Question 22: You have to store those nanmes in a new list whose length of name is odd store the names in uppper case and if the length the name is even then store the names in lower cas"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 40,
   "id": "838a5c00",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "['himanshu',\n",
       " 'SWAGATH',\n",
       " 'VIJAY',\n",
       " 'gaya',\n",
       " 'siddhant',\n",
       " 'pavithra',\n",
       " 'dhivya',\n",
       " 'chetan',\n",
       " 'BILAL',\n",
       " 'YASHWANTH',\n",
       " 'yash',\n",
       " 'jyothi',\n",
       " 'SHINY',\n",
       " 'KAJOL',\n",
       " 'jaspreet',\n",
       " 'SHANKAR',\n",
       " 'rasika',\n",
       " 'AKASH',\n",
       " 'satyajit']"
      ]
     },
     "execution_count": 40,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "names = ['Himanshu','Swagath','Vijay','Gaya','Siddhant','Pavithra','Dhivya','Chetan','Bilal','Yashwanth','Yash','Jyothi','Shiny','Kajol','Jaspreet','Shankar','Rasika','Akash','Satyajit']\n",
    "n=[]\n",
    "n = [name.upper() if len(name) %2!=0 else name.lower()  for name in names]\n",
    "n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "03160dd8",
   "metadata": {},
   "source": [
    "# DICTIONARY:\n",
    "In Python, a dictionary is a versatile and mutable data structure that stores key-value pairs. Unlike sequences (such as lists and tuples) that are indexed by a range of numbers, dictionaries are indexed by keys, which can be of any immutable data type, such as strings, numbers, or tuples. Dictionaries are defined by enclosing comma-separated key-value pairs within curly braces {}"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "cea1466c",
   "metadata": {},
   "source": [
    "# Question 23: how do you access the value with a key in a dictionary?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 8,
   "id": "91d7b0ee",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "John\n",
      "20\n"
     ]
    }
   ],
   "source": [
    "my_dict={'name':'John','age':20,'city':'United states'}\n",
    "print(my_dict['name'])\n",
    "print(my_dict['age'])"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "e28981dc",
   "metadata": {},
   "source": [
    "# Question 24 :how do you change the value associated with key in dictionary?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "id": "ea5d8762",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "31\n"
     ]
    }
   ],
   "source": [
    "my_dict={'name':'John','age':20,'city':'United states'}\n",
    "my_dict['age']=31\n",
    "print(my_dict['age'])"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "249cb9fc",
   "metadata": {},
   "source": [
    "# SET IN PYTHON:\n",
    "\n",
    "In Python, a set is an unordered collection of unique elements. Sets are defined by enclosing comma-separated values within curly braces {}. Sets do not allow duplicate elements, and they do not maintain the order of elements like lists or tuples. Sets are primarily used for membership testing and eliminating duplicate entries."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "6afb49d6",
   "metadata": {},
   "source": [
    "# Question 25: How do you create a set and then you have mix it"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 49,
   "id": "fa3cf6a5",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "{1, 2, 3, 4, 5}\n",
      "{1, 3.14, 'hello'}\n"
     ]
    }
   ],
   "source": [
    "my_set = {1, 2, 3, 4, 5}\n",
    "print(my_set)  \n",
    "\n",
    "mixed_set = {1, \"hello\", True, 3.14}\n",
    "print(mixed_set)  \n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 50,
   "id": "b264fdb5",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "{1, 2, 3, 4, 5, 6}\n",
      "{1, 2, 4, 5, 6}\n"
     ]
    }
   ],
   "source": [
    "my_set.add(6)\n",
    "print(my_set)  \n",
    "\n",
    "my_set.remove(3)\n",
    "print(my_set)  \n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "6b1d765c",
   "metadata": {},
   "source": [
    "# Question 26: Perform the union ,intersection,differenece,symmetric difference on two sets"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 11,
   "id": "9ee8a80a",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "{1, 2, 3, 4, 5}\n",
      "{3}\n",
      "{1, 2}\n",
      "{1, 2, 4, 5}\n"
     ]
    }
   ],
   "source": [
    "set1 = {1, 2, 3}\n",
    "set2 = {3, 4, 5}\n",
    "\n",
    "# Union\n",
    "union_set = set1 | set2\n",
    "print(union_set)  \n",
    "\n",
    "# Intersection\n",
    "intersection_set = set1 & set2\n",
    "print(intersection_set)  \n",
    "\n",
    "# Difference\n",
    "difference_set = set1 - set2\n",
    "print(difference_set)  \n",
    "\n",
    "# Symmetric Difference\n",
    "symmetric_difference_set = set1 ^ set2\n",
    "print(symmetric_difference_set)  \n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "81bf585d",
   "metadata": {},
   "source": [
    "# FUNCTION\n",
    "In Python, a function is a block of reusable code that performs a specific task. Functions allow you to break down your program into smaller, more manageable pieces, making your code more organized, easier to understand, and reusable. Python provides many built-in functions, but you can also create your own custom functions to suit your specific needs."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "87ea9b58",
   "metadata": {},
   "source": [
    "#  Question 27 :How do you create a udf which gives the average of 6 random numbers"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 55,
   "id": "931d922d",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[21, 26, 31, 36, 41, 46, 51, 56, 61, 66, 71, 76, 81, 86, 91, 96, 101, 106, 111, 116, 121, 126, 131, 136, 141, 146, 151, 156, 161, 166, 171, 176, 181, 186, 191, 196, 201, 206, 211, 216, 221, 226, 231]\n"
     ]
    }
   ],
   "source": [
    "l = list(range(21,233,5))\n",
    "len(l)\n",
    "print(l)\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 57,
   "id": "f690f7dc",
   "metadata": {},
   "outputs": [],
   "source": [
    "def avg_n(*args):\n",
    "    return int(sum(args)/len(args))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 59,
   "id": "0cbd955c",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "126"
      ]
     },
     "execution_count": 59,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "avg_n(21, 26, 31, 36, 41, 46, 51, 56, 61, 66, 71, 76, 81, 86, 91, 96, 101, 106, 111, 116, 121, 126, 131, 136, 141, 146, 151, 156, 161, 166, 171, 176, 181, 186, 191, 196, 201, 206, 211, 216, 221, 226, 231)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "8c6566ac",
   "metadata": {},
   "source": [
    "# Question 28 :createe a udf which takes a username as an inout and a passsword as input and your fav queston as an input\n",
    "#user name shouls be the name for eg himanshu\n",
    "#password can be aplhanumberic for captain@13143\n",
    "#username:badmorning\n",
    "#passwors:gotohell\n",
    "#what is your boss name?:monkey\n",
    "    #if the password and username and question matches:\n",
    "        #print(\"welcom to lab\")\n",
    "       # else:\n",
    "      #      print(\"inavlid  user entered ...security alarms acivated\")\n",
    "        "
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 12,
   "id": "f5d879b7",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter your name:ak\n",
      " Enter the password:goto heaven\n",
      "what is your fav animal:dog\n"
     ]
    }
   ],
   "source": [
    "username=input(\"Enter your name:\")\n",
    "password=input(\" Enter the password:\")\n",
    "question=input(\"what is your fav animal:\")\n",
    "def cyber_security(u,p,q):\n",
    "    if u == \"akash\" and p==\"gotohell\" and q==\"tiger\":\n",
    "        print(\"hi\",u,\"welcome to the lab\")\n",
    "    else:\n",
    "        print(\"invalid user entered .....security alarms activated\")\n",
    "    \n",
    "    \n",
    "         \n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 13,
   "id": "db4fd6d0",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "invalid user entered .....security alarms activated\n"
     ]
    }
   ],
   "source": [
    "cyber_security(username,password,question) "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "b1743d18",
   "metadata": {},
   "source": [
    "# Question 29:How do you create a udf gives factorial of any number?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 14,
   "id": "a1e5a8fd",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "120"
      ]
     },
     "execution_count": 14,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "\n",
    "def factorial(n):\n",
    "    if n==0 or n==1:\n",
    "        return 1\n",
    "    else:\n",
    "        result=n*factorial(n-1)\n",
    "        return result\n",
    "\n",
    "factorial(5)    "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "1aa29b89",
   "metadata": {},
   "source": [
    "# Question 30: How do you find the greatest n digit number divisble by n?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 66,
   "id": "0c706084",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "99995"
      ]
     },
     "execution_count": 66,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "\n",
    "def greatest_N(n): \n",
    "    G=pow(10,n)-1\n",
    "    L=pow(10,n-1)\n",
    "    l=[]\n",
    "    for i in range(G,L,-1):\n",
    "        if i % n==0:\n",
    "            l.append(i)\n",
    "    return l[0]\n",
    "\n",
    "greatest_N(5)\n",
    "        "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "2062aa86",
   "metadata": {},
   "source": [
    "# Question 31: How do you find the samllest n digit number divisible by N"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 67,
   "id": "1b67fa6c",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "1000"
      ]
     },
     "execution_count": 67,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "#2:find the samllest n digit number divisible by N\n",
    "def smallest_N(n):\n",
    "    G=pow(10,n)-1\n",
    "    L=pow(10,n-1)\n",
    "    l=[]\n",
    "    for i in range(L,G):\n",
    "        if i %n==0: \n",
    "            l.append(i)\n",
    "    return l[0]\n",
    "smallest_N(4)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "c8dd3b3f",
   "metadata": {},
   "source": [
    "# LAMBDA FUNCTION:\n",
    "In Python, a lambda function, also known as an anonymous function or a lambda expression, is a small, inline function that does not have a name. Lambda functions are useful for writing short, one-line functions without the need to define a formal function using the def keyword."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "9b7b4a32",
   "metadata": {},
   "source": [
    "# Question 32: Using the lambda, you have to get the floor value of each of the value given in the original list"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 15,
   "id": "af49f2de",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[23, 34, 60, 27, 14, 9, 15]\n"
     ]
    }
   ],
   "source": [
    "data = [23.456,34.987,60.2826,27.2727,14.3898,9.2272,15.878937] \n",
    "\n",
    "new_data = list(map(lambda x: int(x) if x >= 0 else int(x) - 1, data))\n",
    "print(new_data)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "741e60f2",
   "metadata": {},
   "source": [
    "#   Question 33:Get those even values which are greater than 50 from the list using lambda function."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 21,
   "id": "5bc8c97b",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[60, 72, 84]"
      ]
     },
     "execution_count": 21,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "F = [12,35,25,39,33,45,48,60,72,77,84,91,3,21]\n",
    "f=list(filter(lambda x: x > 50 and x%2==0 ,F))\n",
    "f"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "151907e0",
   "metadata": {},
   "source": [
    "# CLASSES AND OBJECTS IN PYTHON:\n",
    "    In Python, a class is a blueprint for creating objects, and an object is an instance of a class. Classes define the attributes (data) and methods (functions) that characterize the objects created from them. Using classes and objects allows you to create reusable code with clear structure and organization."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "e4a0290b",
   "metadata": {},
   "source": [
    "#  Question 34 :How do you create a simple class in Python?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 72,
   "id": "317c9fcd",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "'Virat Kohli is cricketer whose age is 36.'"
      ]
     },
     "execution_count": 72,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "class Cricket:\n",
    "    name=\"Virat Kohli\" # attribut/insatnce variables/data members\n",
    "    age=36\n",
    "    def show_info(self): #non,parameterized\n",
    "        return f\"{self.name} is cricketer whose age is {self.age}.\"\n",
    "\n",
    "    \n",
    "obj=Cricket()\n",
    "obj.show_info()"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "6fc7854c",
   "metadata": {},
   "source": [
    "# Question 35: Create a class Rectangle with attributes width and height ,Implement methods to calculate the area and perimeter of rectangle\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "id": "19bda035",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "area 20\n",
      "perimeter 18\n"
     ]
    }
   ],
   "source": [
    "class Rectangle:\n",
    "    def __init__(self,width,height):\n",
    "        self.width=width\n",
    "        self.height=height\n",
    "    \n",
    "    def area(self):\n",
    "        return self.width * self.height\n",
    "    \n",
    "    def perimeter(self):\n",
    "        return 2 * (self.width + self.height)\n",
    "        \n",
    "rect = Rectangle(4,5)\n",
    "print(\"area\",rect.area())\n",
    "print(\"perimeter\",rect.perimeter())"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "26fc51a7",
   "metadata": {},
   "source": [
    "# INHERITANCE:\n",
    "Inheritance is a fundamental concept in object-oriented programming (OOP) that allows you to create a new class (called a subclass or derived class) based on an existing class (called a superclass or base class)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "21d6c63f",
   "metadata": {},
   "source": [
    "# Question 36: what is class inheritance and how can you create a subclass in python"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 74,
   "id": "09aa184b",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Black car with LED headlights.\n"
     ]
    }
   ],
   "source": [
    "class Car:\n",
    "    color='Black'\n",
    "    head='LED'\n",
    "    def display_features(self):\n",
    "        print(f\"{self.color} car with {self.head} headlights.\")\n",
    "        \n",
    "        \n",
    "class Kia(Car):\n",
    "    def kia_features(self):\n",
    "        print(\"Kia has Advance features\")\n",
    "        \n",
    "        \n",
    "obj1=Kia()\n",
    "obj1.display_features()"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "3952a0fc",
   "metadata": {},
   "source": [
    "# Question 37 : another example"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 75,
   "id": "ac354fb4",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "'Evening'"
      ]
     },
     "execution_count": 75,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "class A:\n",
    "    def task1(self):\n",
    "        return \"Evening\"\n",
    "class B(A):   \n",
    "    def task2(self):\n",
    "        return \"Morning\"\n",
    "obj2=B()\n",
    "obj2.task1()"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "6faa9e92",
   "metadata": {},
   "source": [
    "# MULTIPLE INHERITANCE:\n",
    "    \n",
    "Multiple inheritance is a feature in object-oriented programming languages like Python that allows a class to inherit attributes and methods from multiple parent classes. This means that a subclass can inherit from more than one superclass."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "9dab988d",
   "metadata": {},
   "source": [
    "# Question 38 : Creating a class of bank related to each other"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 76,
   "id": "e268b1b6",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Patel Nagar Branch\n"
     ]
    }
   ],
   "source": [
    "class OBC:\n",
    "    def branch(self):\n",
    "        print (\"Patel Nagar Branch\")\n",
    "        \n",
    "class Unity_Bank:\n",
    "    def branch(self):\n",
    "        print(\"Nehru Nagar Branch\")\n",
    "        \n",
    "class PNP(OBC,Unity_Bank):\n",
    "    def branch1(self):\n",
    "        print(\"Merger OF  OBC and Unity banl\")\n",
    "n=PNP()\n",
    "n.branch()"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "37b923ea",
   "metadata": {},
   "source": [
    "# Question 39: creating a class of school in which student studies"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 77,
   "id": "9dc0f45f",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "' the name of student is satya and the age is 14 yrs old and the id is 1244'"
      ]
     },
     "execution_count": 77,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "#multiple inheritance\n",
    "class School():\n",
    "    def display_info(self):\n",
    "        return (f\"the name is {self.name}\")\n",
    "\n",
    "class student(School):\n",
    "    def get_info(self):\n",
    "        return (f\" the name of student is satya and the age is 14 yrs old and the id is 1244\")\n",
    "                        \n",
    "Inf=student()\n",
    "Inf.get_info()"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "258b3e0a",
   "metadata": {},
   "source": [
    "# MULTILEVEL INHERITANCE:\n",
    "\n",
    "Multilevel inheritance is a type of inheritance in object-oriented programming where a subclass inherits from another subclass, creating a chain of inheritance. This means that a subclass can act as both a superclass and a subclass, allowing for a hierarchical organization of classes."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "29a67b87",
   "metadata": {},
   "source": [
    "# Question 40: how do you create a class of country in which the state and city are related"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 79,
   "id": "fec2c386",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "'India'"
      ]
     },
     "execution_count": 79,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "class Country:\n",
    "    def task1(self):\n",
    "        return \"India\"\n",
    "    \n",
    "class State(Country):\n",
    "    def task2(self):\n",
    "        return \"Uttarpradesh\"\n",
    "    \n",
    "class City(State):\n",
    "    def task3(self):\n",
    "        return \"NOida\"\n",
    "     \n",
    "    \n",
    "s1=City()\n",
    "s1.task1()"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "894bc786",
   "metadata": {},
   "source": [
    "# OBJECTIVES:"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "c1a321c8",
   "metadata": {},
   "source": [
    "# Question 41 :Write a Python Program to Display the Multiplication Table Using while-loop"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 80,
   "id": "1c1cb355",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter a number: 35\n",
      "35 X 1 = 35\n",
      "35 X 2 = 70\n",
      "35 X 3 = 105\n",
      "35 X 4 = 140\n",
      "35 X 5 = 175\n",
      "35 X 6 = 210\n",
      "35 X 7 = 245\n",
      "35 X 8 = 280\n",
      "35 X 9 = 315\n",
      "35 X 10 = 350\n"
     ]
    }
   ],
   "source": [
    "num = int(input(\"Enter a number: \"))\n",
    "\n",
    "i = 1  # initialization\n",
    "while i<=10:\n",
    "    print(f\"{num} X {i} = {num*i}\")\n",
    "    i+=1"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "960e6f50",
   "metadata": {},
   "source": [
    "#  Question 42 :wirte a Python Program to Sort Words in Alphabetic Order"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 84,
   "id": "efbace3c",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter your sentence: This is Python progam\n",
      "Sorted words:\n",
      "is progam python this\n"
     ]
    }
   ],
   "source": [
    "words = input(\"Enter your sentence: \")\n",
    "\n",
    "# Transform it into lowercase\n",
    "words = words.lower()\n",
    "\n",
    "# Split words into Python list\n",
    "words_list = words.split()\n",
    "\n",
    "# sort words_list\n",
    "words_list.sort()\n",
    "\n",
    "# join sorted_list into single string\n",
    "sorted_words = \" \".join(words_list)\n",
    "\n",
    "print(\"Sorted words:\")\n",
    "print(sorted_words)\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "ff076c1d",
   "metadata": {},
   "source": [
    "# Question 43: Write a program  Convert Celsius to Fahrenheit in Python"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 86,
   "id": "7dc202d5",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter Temperature in Celsius: 36\n",
      "Temperature in Fahrenheit: 96.80 F\n"
     ]
    }
   ],
   "source": [
    "c = float(input(\"Enter Temperature in Celsius: \"))\n",
    "f = (c*(9/5))+32\n",
    "print(f\"Temperature in Fahrenheit: {f:.2f} F\")"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "2d3c49ee",
   "metadata": {},
   "source": [
    "#  Question 44 :How to Convert Decimal to Binary in Python"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 88,
   "id": "a61e00ee",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter a number:10\n",
      "Binary of given number is 1010"
     ]
    }
   ],
   "source": [
    "#How to Convert Decimal to Binary in Python\n",
    "n = int(input(\"Enter a number:\"))\n",
    "# Create a Empty list to store binary numbers\n",
    "binary_list = []\n",
    "# store remainders using while loop\n",
    "while n!=0:\n",
    "    rem = n%2\n",
    "    binary_list.append(rem)\n",
    "    n = n//2\n",
    "\n",
    "# Reverse a list\n",
    "binary_list = binary_list[::-1]\n",
    "\n",
    "# print binary numbers\n",
    "print(\"Binary of given number is \",end='')\n",
    "for num in binary_list:\n",
    "    print(num, end='')"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "f65757aa",
   "metadata": {},
   "source": [
    "# Question 45: Write a python program  to check for vowels."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 92,
   "id": "3d6febfd",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "enter letter to check vowel or not  : v\n",
      "not vowel (consonants)\n"
     ]
    }
   ],
   "source": [
    "string = input(\"enter letter to check vowel or not  : \")\n",
    "string = string.lower()\n",
    "\n",
    "if len(string)<2:\n",
    "    if string == 'a' or string == 'e' or string == 'i' or string == 'o' or string == 'u':\n",
    "        print(f\"{string.upper()} is vowel\")\n",
    "    else:\n",
    "        print(\"not vowel (consonants)\")\n",
    "else:\n",
    "    print(\"enter only one letter  \")"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "d9319395",
   "metadata": {},
   "source": [
    "# Question 46: Write a python program to check the given year is leap year or not."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 93,
   "id": "4703ab41",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter your Year: 2022\n",
      "2022 is Not a Leap year\n"
     ]
    }
   ],
   "source": [
    "year = int(input('Enter your Year: '))\n",
    "\n",
    "if year % 4 == 0:\n",
    "    if year % 100 == 0:\n",
    "        if year % 400 ==0:\n",
    "            print(f\"{year} is a Leap year\")\n",
    "        else:\n",
    "            print(f\"{year} is Not a Leap year\")\n",
    "    else:\n",
    "        print(f\"{year} is a Leap year\")\n",
    "else:\n",
    "    print(f\"{year} is Not a Leap year\")"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "415374d4",
   "metadata": {},
   "source": [
    "# Question 47: Write a Python Program to Calculate Area of Rectangle"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 94,
   "id": "3259c4e3",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter Length of the Rectangle: 4\n",
      "Enter Breadth of the Rectangle: 5\n",
      "Area of rectangle is 20.00\n"
     ]
    }
   ],
   "source": [
    "\n",
    "l = float(input('Enter Length of the Rectangle: '))\n",
    "b = float(input('Enter Breadth of the Rectangle: '))\n",
    "\n",
    "area = l * b\n",
    "\n",
    "print(f\"Area of rectangle is {area:.2f}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "b6670966",
   "metadata": {},
   "source": [
    "# Question 48: Write a Python Program to Convert Kilometers to Miles"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 95,
   "id": "4b38480c",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter value in KMs: 5\n",
      "5 kms will be 3.106855 Miles\n"
     ]
    }
   ],
   "source": [
    "\n",
    "km = int(input(\"Enter value in KMs: \"))\n",
    "\n",
    "miles = km * 0.621371\n",
    "print(f\"{km} kms will be {miles} Miles\")"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "90b863fc",
   "metadata": {},
   "source": [
    "# Question 49: Write a Simple Interest Program in Python taking random values"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 97,
   "id": "0ea7f33c",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter Principal Amount: 5000\n",
      "Enter Rate of Interest: 10\n",
      "Enter Time Period: 3\n",
      "Simple Interest is: 1500.0\n"
     ]
    }
   ],
   "source": [
    "p = int(input(\"Enter Principal Amount: \"))\n",
    "r = int(input(\"Enter Rate of Interest: \"))\n",
    "t = int(input(\"Enter Time Period: \"))\n",
    "\n",
    "simple_interest = (p*r*t)/100\n",
    "\n",
    "print(f\"Simple Interest is: {simple_interest}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "9514a0ab",
   "metadata": {},
   "source": [
    "# Pattern programs in python"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "4579fdfe",
   "metadata": {},
   "source": [
    "# Question 50: Write a python to get left triangle pattern"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 98,
   "id": "935b5bd8",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter length of the pattern: 5\n",
      "*\n",
      "**\n",
      "***\n",
      "****\n",
      "*****\n"
     ]
    }
   ],
   "source": [
    "\n",
    "\n",
    "length = int(input('Enter length of the pattern: '))\n",
    "\n",
    "for i in range(length):\n",
    "    for j in range(i+1):\n",
    "        print('*',end='')\n",
    "    print()  # for new line"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a4a93e0e",
   "metadata": {},
   "source": [
    "# Question 51:creating a quz game using basic python"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "id": "e98a183f",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Wellcome to quiz game !!\n",
      "NOTE: if your spelling is incorrect then it is considered as wrong answer\n",
      "Do you want to play ? yes\n",
      "\n",
      "1. what does CPU stand for? central processing unit\n",
      "correct! you got 1 point\n",
      "\n",
      "2. what does GPU stand for? get et\n",
      "Incorrect!\n",
      "current answer is --> graphics processing unit\n",
      "\n",
      "3. what does RAM stand for? random acesss memory\n",
      "Incorrect!\n",
      "current answer is --> random access memory\n",
      "\n",
      "4. what does PSU stand for? power supply unit\n",
      "correct! you got 1 point\n",
      "\n",
      "5. what does ROM stand for? read only memory\n",
      "correct! you got 1 point\n",
      "\n",
      "number of question is 5\n",
      "your score is 3\n",
      "60.0% questions are correct.\n"
     ]
    }
   ],
   "source": [
    "#Create a sim\n",
    "print(\"Wellcome to quiz game !!\")\n",
    "print('NOTE: if your spelling is incorrect then it is considered as wrong answer')\n",
    "score = 0\n",
    "question_no = 0\n",
    "playing = input('Do you want to play ? ').lower()\n",
    "if playing == 'yes':\n",
    "    question_no += 1\n",
    "    ques = input(f'\\n{question_no}. what does CPU stand for? ').lower()\n",
    "    if ques == 'central processing unit':\n",
    "        score +=1\n",
    "        print('correct! you got 1 point')\n",
    "        \n",
    "    else:\n",
    "        print('Incorrect!')\n",
    "        print(f'current answer is --> central processing unit')\n",
    "\n",
    "# ------1\n",
    "    question_no += 1\n",
    "    ques = input(f'\\n{question_no}. what does GPU stand for? ').lower()\n",
    "    \n",
    "    if ques == 'graphics processing unit':\n",
    "        score +=1\n",
    "        print('correct! you got 1 point')\n",
    "        \n",
    "    else:\n",
    "        print('Incorrect!')\n",
    "        print(f'current answer is --> graphics processing unit')\n",
    "\n",
    "# -----2\n",
    "    question_no += 1\n",
    "    ques = input(f'\\n{question_no}. what does RAM stand for? ').lower()\n",
    "    \n",
    "    if ques == 'random access memory':\n",
    "        score +=1\n",
    "        print('correct! you got 1 point')\n",
    "        \n",
    "    else:\n",
    "        print('Incorrect!')\n",
    "        print(f'current answer is --> random access memory')\n",
    "\n",
    "# -----3\n",
    "    question_no += 1\n",
    "    ques = input(f'\\n{question_no}. what does PSU stand for? ').lower()\n",
    "    \n",
    "    if ques == 'power supply unit':\n",
    "        score +=1\n",
    "        print('correct! you got 1 point')\n",
    "        \n",
    "    else:\n",
    "        print('Incorrect!')\n",
    "        print(f'current answer is --> power supply unit')\n",
    "\n",
    "\n",
    "# -----4\n",
    "    question_no += 1\n",
    "    ques = input(f'\\n{question_no}. what does ROM stand for? ').lower()\n",
    "    \n",
    "    if ques == 'read only memory':\n",
    "        score +=1\n",
    "        print('correct! you got 1 point')\n",
    "        \n",
    "    else:\n",
    "        print('Incorrect!')\n",
    "        print(f'current answer is --> read only memory')\n",
    "\n",
    "\n",
    "# ------5 \n",
    "\n",
    "else:\n",
    "    print('thankyou you are out of a game.')\n",
    "    quit()\n",
    "\n",
    "print(f'\\nnumber of question is {question_no}')\n",
    "print(f'your score is {score}')\n",
    "try:\n",
    "    percentage = (score *100)/question_no\n",
    "except ZeroDivisionError:\n",
    "    print('0% quetions are correct')\n",
    "\n",
    "print(f'{percentage}% questions are correct.')"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "d4677c89",
   "metadata": {},
   "source": [
    "# Question 52: Write a python Program to calculate Electricity Bill in Python by Taking Input from the User"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "e893d2ed",
   "metadata": {},
   "outputs": [],
   "source": [
    "\n",
    "# 1 to 100 units - 1.5Rs\n",
    "# 101 to 200 units - 2.5Rs\n",
    "# 201 to 300 units - 4Rs\n",
    "# 300 to 350 units - 5Rs\n",
    "# Above 350 - Fixed charge 1500Rs\n",
    "\n",
    "units = float(input(\"Enter the Unit Consumed: \"))\n",
    "\n",
    "if units > 0 and units <= 100:\n",
    "    payment = units * 1.5\n",
    "    fixedCharge = 25 # Extra charge\n",
    "elif units > 100 and units <= 200:\n",
    "    payment = (100 * 1.5) + (units - 100) * 2.5\n",
    "    fixedCharge = 50 # Extra charge\n",
    "elif units > 200 and units <= 300:\n",
    "    payment =  (100 * 1.5) + (200 - 100) * 2.5 + (units - 200) * 4\n",
    "    fixedCharge = 75 # Extra charge\n",
    "elif units > 300 and units <= 350:\n",
    "    payment = (100 * 1.5) + (200 - 100) * 2.5 + (300 - 200) * 4 + (units - 300) * 5   \n",
    "    fixedCharge = 100 # Extra charge\n",
    "else:\n",
    "    payment = 0\n",
    "    fixedCharge = 1500\n",
    "\n",
    "total = payment + fixedCharge\n",
    "\n",
    "print(f\"Your Electricity Bill amount is {total:.2f}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "f941ed5e",
   "metadata": {},
   "source": [
    "#  Question 53 : How to Check if a Number is a Perfect Square in Python"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "id": "d5f892a6",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Enter a Number: 64\n",
      "64 is a Perfect Square\n"
     ]
    }
   ],
   "source": [
    "num = int(input(\"Enter a Number: \"))\n",
    "flag = 0\n",
    "\n",
    "for i in range(1, num+1):\n",
    "    if i*i == num:\n",
    "        flag = 1\n",
    "        break\n",
    "\n",
    "if flag == 1:\n",
    "    print(f\"{num} is a Perfect Square\")\n",
    "else:\n",
    "    print(f\"{num} is not a Perfect Square\")"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "2abf3eec",
   "metadata": {},
   "source": [
    "# Question 54: how do you count the number of females and makes in given list?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "id": "fd34e274",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "number of females 60\n",
      "number of males: 45\n"
     ]
    }
   ],
   "source": [
    "gender = ['Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female','Female','Male','F','M','female','male','Female']\n",
    "if (\"Female\") or(\"F\") or (\"M\") or ('Male') or ('female') or ('male')in gender:\n",
    "    print(\"number of females\",gender.count('Female')+ gender.count('F')+gender.count('female'))\n",
    "    print(\"number of males:\",gender.count('Male')+  gender.count('M')+gender.count('male'))"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "6a0e4cac",
   "metadata": {},
   "source": [
    "# Question 55: You have to get the employees id respected to their company"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "id": "f05785f5",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "TCS: ['TCS101', 'TCS301', 'TCS1101', 'TCS1601']\n",
      "HCL: ['HCL201', 'HCL2201', 'HCL2001', 'HCL6201']\n",
      "COG: ['COG324', 'COG3124', 'COG3214', 'COG3924']\n",
      "IBM: ['IBM322', 'IBM3212', 'IBM3221', 'IBM3228']\n"
     ]
    }
   ],
   "source": [
    "comp = ['TCS101','HCL201','COG324','IBM322','TCS301','HCL2201','COG3124','IBM3212','TCS1101','HCL2001','COG3214','IBM3221','TCS1601','HCL6201','COG3924','IBM3228']\n",
    "TCS=[]\n",
    "HCL=[]\n",
    "COG=[]\n",
    "IBM=[]\n",
    "for i in comp:\n",
    "    if i.startswith('T'):\n",
    "        TCS.append(i)\n",
    "    elif  i.startswith('H'):\n",
    "        HCL.append(i)\n",
    "    elif i.startswith('C'):\n",
    "        COG.append(i)\n",
    "    else:\n",
    "        IBM.append(i)\n",
    "\n",
    "        \n",
    "print(\"TCS:\",TCS)\n",
    "print(\"HCL:\",HCL)\n",
    "print(\"COG:\",COG)\n",
    "print(\"IBM:\",IBM)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "4243ec02",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.13"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
