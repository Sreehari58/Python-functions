# Python-functions
python functions for the freshers..
# ## BUILT-IN FUNCTIONS

# In[1]:


# (1) print()- Outputs to the console
a = 4
b = 7
print(a+b)


# In[3]:


# (2) len()- returns the length of the object
# Define a list of items
my_list = ['apple', 'banana', 'cherry']

# Use len() to get the number of items in the list
list_length = len(my_list)

print("The number of items in the list is:", list_length)

#string length
my_string = 'Hi My name is SREEHARI THIRUMALAI BHUVARAGHAVAN'

#use len() function for the string length
string_length = len(my_string)

print ("the length of the string is :",string_length)


# In[9]:


# (3) type()- Returns the type of the object
# Example demonstrating the type() function

# Integer type
my_int = 7
print("The type of my_int is:", type(my_int))

# Float type
my_float = 7.0
print("The type of my_float is:", type(my_float))

# String type
my_string = "Hello, Python!"
print("The type of my_string is:", type(my_string))

# List type
my_list = [1, 2, 3]
print("The type of my_list is:", type(my_list))

# Dictionary type
my_dict = {'name': 'John', 'age': 30}
print("The type of my_dict is:", type(my_dict))

# Boolean type
my_bool = True
print("The type of my_bool is:", type(my_bool))


# Define variables of different types
a_number = 42
a_string = "Hello!"
a_list = [1, 2, 3]
a_tuple = (4, 5, 6)

# Print out the types of these variables
print("The type of a_number is:", type(a_number))
print("The type of a_string is:", type(a_string))
print("The type of a_list is:", type(a_list))
print("The type of a_tuple is:", type(a_tuple))


# In[17]:


# (4) input()- Reads input from the user
# Ask the user to input their name
name = input("Please enter your name: ")

# Ask the user to input their age
age = input("Please enter your age: ")

# Print a greeting message including the user's name and age
print(f"Hello {name}! You are {age} years old.")

##The f inside the print() statement in Python indicates that the string is a formatted string literal, commonly known as an f-string. F-strings provide a way to embed expressions inside string literals, using curly braces {}. The expressions are evaluated at runtime and formatted using the specified format. This feature was introduced in Python 3.6 and is widely used for its simplicity and readability.

# Ask the user for their favorite color
favorite_color = input("What is your favorite color? ")

# Output a message including the user's favorite color
print(f"Wow, {favorite_color} is a great color!")


# In[18]:


# (5) range() - Generates a sequence of numbers
# Using range() to generate numbers from 0 to 4
for i in range(5):
    print(i)
# Using range() with a negative step to count backwards from 10 to 1
for i in range(10,0,-1):
    print(i)
# Using range() to generate every second number from 2 to 20    
for i in range(2,21,2):
    print(i)


# In[20]:


# (6) enumerate()- Returns an enumerate object (gives the index value of the object in the sequence)
# Define a list of fruits
fruits = ['apple','jack fruit','mango','grapes','orange']
# use enumerate() to loop through the list with an index
for index,fruit in enumerate(fruits):
    print(f"Index {index}: {fruit}")


# In[21]:


# (7) zip() - Combines multiple iterables
#Suppose you have two lists, one with names and another with ages, and you want to pair each name with its corresponding age.
# Define two lists
names = ['Alice', 'Bob', 'Charlie']
ages = [25, 30, 35]

# Use zip() to combine the lists
combined = zip(names, ages)

# Convert the zip object to a list and print it
combined_list = list(combined)
print(combined_list)

#another example 
# Loop through the zipped object
for name, age in zip(names, ages):
    print(f"{name} is {age} years old.")


# In[27]:


# (8) sum() - Calculates the sum of elements
# Define a list of numbers
numbers = [10, 20, 30, 40, 50]

# Use sum() to calculate the total of the numbers in the list
total = sum(numbers)

# Print the total
print("The total is:", total)

a = 5
b = 6
c = a+b
print(c)


# In[28]:


# (9) min()- Returns the smallest item in a iterable

#finding the minimum in the list
# Define a list of numbers
numbers = [50, 20, 40, 10, 30]

# Use min() to find the smallest number in the list
minimum_value = min(numbers)

# Print the smallest number
print("The smallest number is:", minimum_value)

#You can also use the key parameter in min() to specify a function to be called on each list element before making comparisons.
# Define a list of names
names = ["Alice", "Bob", "alexandra", "chris"]

# Use min() to find the smallest name based on the length of the name
shortest_name = min(names, key=len)

# Print the name with the shortest length
print("The name with the shortest length is:", shortest_name)



# In[29]:


# (10) max() - Returns the largest element of the list/ item in an iterable
# Define a list of numbers
numbers = [10, 20, 70, 40, 30]

# Use max() to find the largest number in the list
maximum_value = max(numbers)

# Print the largest number
print("The largest number is:", maximum_value)

#finding the maximum in the list of strings
#Define a list of the strings
words = ["cat","ant","bat","dog"]

#use max() to find the lexicographically largest string
largest_word = max(words)

#print the largest value
print("the lexicographically largest word is:",largest_word)


# In[30]:


#(11) sorted() - Returns the sorted list
# Define a list of numbers
numbers = [50, 20, 80, 40, 10]

# Sort the list of numbers in ascending order
sorted_numbers = sorted(numbers)

# Print the sorted list
print("Sorted numbers:", sorted_numbers)

# Sorting a lsit of strings lexicographically
# Define a list of strings
words = ['Helicopter', 'Rocket', 'Airplane', 'Jet']

# Sort the list of strings
sorted_words = sorted(words)

# Print the sorted list of strings
print("Sorted words:", sorted_words)


#sorting by length of items in a list
# Define a list of names
names = ['SREEHARI', 'USMAN', 'KEWIN', 'SHARATH']

# Sort the names by length
sorted_by_length = sorted(names, key=len)

# Print the names sorted by length
print("Names sorted by length:", sorted_by_length)





# In[31]:


# (12) reversed() - Returns the reversed iterator
#The reversed() function in Python is used to return an iterator that accesses the given sequence in the reverse order. It's particularly useful for reversing lists or any sequence types like tuples and strings, without altering the original sequence.
# Define a list of numbers
numbers = [1, 2, 3, 4, 5]

# Use reversed() to reverse the list
reversed_numbers = reversed(numbers)

# Convert the reversed object to a list and print it
print("Reversed numbers:", list(reversed_numbers))


#another example
# reversing a tuple
#Define a tuple
tup = ('a','b','c','d')
# use reversed() to reverse the tuple
reversed_tuple = reversed(tup)
#Convert the reversed object to a tuple and print it
print("Reversed tuple:",tuple(reversed_tuple))


# In[33]:


# (13) abs() - Returns the absolute value
# An integer with a negative value
negative_number = -10
# Getting the absolute value
absolute_value = abs(negative_number)
#print the result
print("The absolute value of",negative_number,"is",absolute_value)

#absolute value of a complex number
complex_number = 3+4j
# Getting the magnitude (absolute value)
magnitude = abs(complex_number)
#print the result
print("The magnitude of the complex number",complex_number,"is",magnitude)

# another example
#List of mixed negative and positive numbers
numbers = [-1, 2, -3, 4, -5]
# using list comprehension to get absolute values
absolute_numbers = [abs(num) for num in numbers]
# Print the list of absolute values
print("Absolute values:",absolute_numbers)


# In[34]:


# (14) round() - Rounds a number to a specified precision
# A floating-point number
number = 7.5
# Rounding to the nearest integer
rounded_number = round(number)
#Print the result
print("round to the nearest integer:",rounded_number)

#Rounding works similarly with negative numbers
# A negative floating-point number
negative_number = -2.678

# Rounding to one decimal place
rounded_negative = round(negative_number, 1)

# Print the result
print("Rounded negative number:", rounded_negative)


#Rounding and list comprehension
# List of floating-point numbers
numbers = [1.955, 2.505, 3.144, 4.999]

# Rounding all numbers to one decimal place using list comprehension
rounded_numbers = [round(num, 1) for num in numbers]

# Print the rounded numbers
print("Rounded numbers:", rounded_numbers)


# In[35]:


# (15) any() - Returns True if any element is true
# List of boolean values
bool_values = [False, False, True, False]

# Check if any element is True
result = any(bool_values)

# Print the result
print("Is there any True value?:", result)


#another example
# using any() with numbers
# List of numbers
numbers = [0, 0, 0, 0, 1]

# Check if any element is non-zero
result = any(numbers)

# Print the result
print("Is there any non-zero value?:", result)


#another example
# List of strings
strings = ["", "", "hello", ""]

# Check if any string is non-empty
result = any(strings)

# Print the result
print("Is there any non-empty string?:", result)



# In[1]:


# (16) all() - Returns True if all elements are true

# List of boolean values
bool_values = [True, True, False, True]

# Check if all elements are True
result = all(bool_values)

# Print the result
print("Are all values True?:", result)


#Since non-zero numbers are truthy, all() can be used to check if all elements in a list are non-zero:
# List of numbers
numbers = [1, 2, 3, 4, 5]

# Check if all elements are non-zero
result = all(numbers)

# Print the result
print("Are all numbers non-zero?:", result)


# In[3]:


# (17) filter() - Filters the elements based on a function

# Define a list of numbers
numbers = [1, 10, 12, 15, 20, 2, 5, 8]

# Define a function that checks if a number is greater than 10
def is_greater_than_10(num):
    return num > 10

# Use filter() to apply the function
filtered_numbers = filter(is_greater_than_10, numbers)

# Convert filter object to a list and print it
print("Numbers greater than 10:", list(filtered_numbers))

# Define a list of strings
strings = ["apple", "", "banana", None, "cherry", ""]

# Use filter() to remove empty strings
non_empty_strings = filter(None, strings)

# Convert filter object to a list and print it
print("Non-empty strings:", list(non_empty_strings))




# In[17]:


# (18) map() - Applies a function to all the items in an input list

# Define a list of temperatures in Celsius
temperatures_celsius = [0, 10, 20, 30]

# Define a function that converts Celsius to Fahrenheit
def celsius_to_fahrenheit(c):
    return (c * 9/5) + 32

# Use map() to apply the conversion function
temperatures_fahrenheit = map(celsius_to_fahrenheit, temperatures_celsius)

# Convert map object to a list and print it
print("Temperatures in Fahrenheit:", list(temperatures_fahrenheit))


# Define a list of strings
words = ["apple", "banana", "cherry"]

# Use map() to calculate the length of each word
lengths = map(len, words)

# Print the lengths
print("Lengths of words:", list(lengths))



# ## DICTIONARY FUNCTIONS

# In[8]:


# (1) dict() - Creates new dictionary

data_list = [["Name1",'Sreehari'], ["Name2",'Justus'], ["Name3",'Usman']]
data_dict = dict(data_list)

print("Dictionary from data lists:", data_dict)

#Another example
data = [['Sreehari',7010706101], ['Thirumalai',9710013927], ['Hemalatha',9710709769]]
data_dict = dict(data)
print("Dictionary from data:",data_dict)


# In[10]:


# (2) keys() - Returns the keys of a dictionary
# Create a dictionary
person = {'name': 'Sreehari', 'age': 23, 'city': 'Chicago'}

# Get the keys from the dictionary
keys = person.keys()

# Print the keys
print("Keys:", keys)

#another example by continuing
# Iterate over the keys and print each one
for key in person.keys():
    print(key)




# In[8]:


# (3) values() - Returns the values of a dictionary


# Correcting the structure to a list of dictionaries
person_details = [
    {'name': 'Sreehari', 'age': 23, 'city': 'Chicago'},
    {'name': 'Usman', 'age': 22, 'city': 'Chicago'},
    {'name': 'Kewin', 'age': 22, 'city': 'Chicago'}
]

# Using a list comprehension to get all values from each dictionary in the list
values = [person.values() for person in person_details]

# Print the values
print("Values:")
for value in values:
    print(value)
    
#another example
# Create a dictionary
person = {'name': 'Alice', 'age': 25, 'city': 'New York'}

# Get the values from the dictionary
values = person.values()

# Print the values
print("Values:", values)
# Iterate over the values and print each one
for value in person.values():
    print(value)




# In[10]:


# (4) items() - Returns the key-value pairs of a dictionary

# Define a dictionary
inventory = {'apples': 30, 'bananas': 15, 'cherries': 45}

# Use the items() method to access keys and values
for fruit, quantity in inventory.items():
    print(f"There are {quantity} {fruit} in the inventory.")

# another example
steam_engine = {'rockstar_games': 2, 'sports_games': 3, 'Co-op_games':4}
#use the items() method to access keys and values
for games, quantity in steam_engine.items():
    print(f"I have {quantity} {games} in the steam_engine.")


# In[14]:


# (5) get() - Returns the value for a given key

# Define a list of dictionaries where each dictionary contains details of one employee
Employees = [
    {'name': 'Justus', 'age': 22, 'Department': 'Developer-side'},
    {'name': 'Sreehari', 'age': 23, 'Department': 'Data-Analyst'},
    {'name': 'Usman', 'age': 21, 'Department': 'ML-Engineer'}
]

# Print the Department of each employee
for employee in Employees:
    department = employee.get('Department', 'No Department Listed')
    print(f"Department of {employee.get('name')}: {department}")
    
#another example
# Define a dictionary
employee = {'name': 'John', 'age': 28, 'department': 'Marketing'}

# Use the get() method to retrieve the age
age = employee.get('age')
print("Age of the employee:", age)

# Attempt to retrieve a key that does not exist, using get()
salary = employee.get('salary', 'Not available')
print("Salary of the employee:", salary)



# In[18]:


# (6) pop() - Removes and returns the value for a given key

# Define a list of numbers
numbers = [10, 20, 30, 40, 50]

# Pop the third element (index 2)
popped_item = numbers.pop(2)

# Print the popped item
print("Popped item:", popped_item)

# Print the list after popping
print("List after popping:", numbers)


# another example

# Define a dictionary
person = {'name': 'Alice', 'age': 25, 'city': 'New York'}

# Pop the 'age' element
popped_age = person.pop('age')

# Print the popped item
print("Popped age:", popped_age)

# Print the dictionary after popping
print("Dictionary after popping:", person)



# In[20]:


# (7) update() - Updates a dictionary with key-value pairs from another dictionary

# Define the first dictionary
employee = {'name': 'Sreehari', 'age': 23, 'department': 'Computer-science-Engineering'}

# Define the second dictionary with updates
updates = {'age': 22, 'city': 'Chicago', 'department': 'CSE'}

# Use the update() method to merge the updates into the employee dictionary
employee.update(updates)

# Print the updated dictionary
print("Updated employee details:", employee)

# Define the first dictionary
fruit = {'name': 'Orange', 'color': 'blue', 'taste': 'salty'}

# Define the second dictionary with updates
updates = {'life-span': 50, 'color': 'orange', 'taste': 'sweet-sour'}

# Use the update() method to merge the updates into the employee dictionary
fruit.update(updates)

# Print the updated dictionary
print("Updated fruit details:", fruit)


# In[21]:


# (8) clear() - Removes all items from the dictionary
#The clear() function in Python is used with dictionaries, lists, and sets to remove all items from the collection, leaving it empty.

# Define a dictionary with some initial data
info = {'name': 'John', 'age': 30, 'city': 'New York'}

# Print the original dictionary
print("Original dictionary:", info)

# Use the clear() method to remove all items
info.clear()

# Print the dictionary after using clear()
print("Dictionary after clear():", info)




# In[22]:


# (9) copy() - returns a shallow copy of the dictionary

# Define a dictionary
original_dict = {'name': 'Alice', 'age': 30, 'skills': ['Python', 'Data Analysis']}

# Make a shallow copy of the dictionary
copied_dict = original_dict.copy()

# Print the original dictionary
print("Original dictionary:", original_dict)

# Print the copied dictionary
print("Copied dictionary:", copied_dict)

# Modify a mutable element in the copied dictionary
copied_dict['skills'].append('Machine Learning')

# Print the original dictionary after modifying the copied one
print("Original dictionary after modifying the copy:", original_dict)



# In[24]:


# (10) fromkeys() - Creates a new dictionary with keys from a sequence and values set to a default value.
#The fromkeys() method in Python is a class method available on dictionary objects that is used to create a new dictionary from a given sequence of keys, with all values set to a specified value. This method is particularly useful when you need to initialize a dictionary with keys, all having the same default value.

# Define a list of keys
keys = ['a', 'b', 'c', 'd']

# Initialize the dictionary from keys with a default value of 0
new_dict = dict.fromkeys(keys, 0)

# Print the new dictionary
print("New Dictionary:", new_dict)

# another example

# Define a list of student names
students = ['Alice', 'Bob', 'Charlie', 'Diana']

# Initialize the attendance dictionary with all students marked as not present
attendance = dict.fromkeys(students, False)

# Print the initial attendance status
print("Initial attendance:", attendance)

# Mark Charlie as present
attendance['Charlie'] = True

# Print the updated attendance status
print("Updated attendance:", attendance)



# # STRING FUNCTIONS

# In[1]:


# (1) str() - Converts an object to a string

# Define a list
fruits = ['apple', 'banana', 'cherry']

# Convert the list to a string
fruits_str = str(fruits)

# Print the string representation of the list
print("String representation of fruits:", fruits_str)

# Define an integer and a string
age = 30
message = "John is " + str(age) + " years old."

# Print the message
print(message)



# In[2]:


# (2) format() - formats a string

#The format() function in Python is used for string formatting. It allows you to construct strings by substituting parts of the strings with data stored in variables. This function is versatile, supporting multiple methods to insert values into a string template. It can be especially useful for creating strings that include numbers, dates, or automatically formatted data.

# Define variables
name = "Alice"
age = 30

# Use format to substitute variables into the string
message = "My name is {} and I am {} years old.".format(name, age)

# Print the formatted message
print(message)


# Formatting floating point numbers
salary = 485000.3333

# Format to two decimal places
formatted_salary = "Your salary is ${:.2f}".format(salary)

# Print formatted salary
print(formatted_salary)




# In[3]:


# (3) split() - splits a string into a list

#The split() function in Python is a string method used to divide a string into a list of substrates based on a specified separator. If no separator is specified, the method defaults to splitting at whitespace, which includes spaces, tabs, and line breaks.

# Define a string with comma-separated values
data = "apple,banana,cherry,grape"

# Split the string at each comma
fruits = data.split(',')

# Print the list of fruits
print("Fruits:", fruits)

# Define a multiline string
paragraph = "Hello world!\nWelcome to Python.\nEnjoy learning!"

# Split the string at newlines
lines = paragraph.split('\n')

# Print the list of lines
print("Lines:", lines)




# In[4]:


# (4) join() - joins elements of a list into a string

# Define a list of words
words = ['Python', 'is', 'awesome', 'for', 'programming']

# Join the words with a space as the separator
sentence = ' '.join(words)

# Print the joined sentence
print("Joined sentence:", sentence)



# Define a list of data items
data = ['apple', 'banana', 'cherry']

# Join the items with a comma and space as the separator
csv_line = ', '.join(data)

# Print the CSV line
print("CSV line:", csv_line)



# In[1]:


# (5) strip() - Removes leading/trailing characters

# Define a string with leading and trailing whitespace
text = "   Hello, Python!   "

# Use strip() to remove the whitespace
clean_text = text.strip()

# Print the original and cleaned text
print("Original text:", repr(text))
print("Cleaned text:", repr(clean_text))


# Define a string with specific characters on both ends
url = "www.example.com////"

# Use strip() to remove the slashes
clean_url = url.strip('/')

# Print the original and cleaned URL
print("Original URL:", repr(url))
print("Cleaned URL:", repr(clean_url))



# In[1]:


# (6) replace() - Replaces substrings in a string

# Define a string
text = "Hello, world! Welcome to this world!"

# Use replace() to change 'world' to 'universe'
modified_text = text.replace("world", "universe")

# Print the modified text
print("Modified text:", modified_text)



# Define a multiline string
multiline_text = "Hello,\nPython\nWorld!"

# Replace newline characters with spaces
single_line_text = multiline_text.replace("\n", " ")

# Print the single line text
print("Single line text:", single_line_text)



# In[2]:


# (7) lower() - converts a string to lowercase

# Define a string
text = "Hello, Python World!"

# Use lower() to convert the string to lowercase
lower_text = text.lower()

# Print the lowercase text
print("Lowercase text:", lower_text)

# Define a list of strings
titles = ["Mr.", "MRS.", "Dr.", "ms."]

# Convert all titles to lowercase
normalized_titles = [title.lower() for title in titles]

# Print the normalized titles
print("Normalized titles:", normalized_titles)


# In[3]:


# (8) upper() - Converts a string to uppercase

# Define a string
text = "Hello, Python World!"

# Use upper() to convert the string to uppercase
upper_text = text.upper()

# Print the uppercase text
print("Uppercase text:", upper_text)

# Define a warning message
warning = "caution: wet floor"

# Convert to uppercase to emphasize the warning
emphasized_warning = warning.upper()

# Print the emphasized warning
print("Warning:", emphasized_warning)


# In[4]:


# (9) startswith() - checks if a string starts with a specified substring

# Define a string
filename = "example.txt"

# Check if the string starts with 'example'
if filename.startswith("example"):
    print("The filename starts with 'example'.")
else:
    print("The filename does not start with 'example'.")


# Define a string
sentence = "Python is easy to learn."

# Check if the part of the string starting at index 10 starts with 'easy'
if sentence.startswith("easy", 10):
    print("The substring starting at index 10 is 'easy'.")
else:
    print("The substring starting at index 10 is not 'easy'.")



# In[5]:


# (10) endswith() - checks if a string ends with a specified substring

# Define a string
filename = "report.pdf"

# Check if the string ends with '.pdf'
if filename.endswith(".pdf"):
    print("The file is a PDF document.")
else:
    print("The file is not a PDF document.")



# Define a string
image_file = "photo.jpeg"

# Check if the file name ends with any of several common image file extensions
if image_file.endswith((".png", ".jpg", ".jpeg", ".gif", ".bmp")):
    print("The file is an image.")
else:
    print("The file is not an image.")


# In[7]:


# (11) isdigit() - checks if all characters are digits

# Define a string
number = "12345"

# Use isdigit to check if the string is numeric
if number.isdigit():
    print("The string is numeric.")
else:
    print("The string contains non-numeric characters.")

# Get user input
user_input = input("Please enter a number: ")

# Validate if the input is a digit
if user_input.isdigit():
    print("Thank you for entering a number.")
else:
    print("Error: You did not enter a valid number.")



# In[8]:


# (12) isalpha() - checks if all characters are alphabetic

# Define a string
text = "Hello"

# Use isalpha to check if the string is alphabetic
if text.isalpha():
    print("The string is alphabetic.")
else:
    print("The string contains non-alphabetic characters.")

# Get user input
user_input = input("Please enter your first name: ")

# Validate if the input is alphabetic
if user_input.isalpha():
    print("Thank you for entering your name.")
else:
    print("Error: The name should not include numbers or special characters.")
