# Creating a dictionary
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}

# Accessing values using keys
print("Name:", my_dict['name'])  # Output: John
print("Age:", my_dict['age'])    # Output: 25
print("City:", my_dict['city'])  # Output: New York

# Adding a new key-value pair
my_dict['occupation'] = 'Engineer'
print("Occupation:", my_dict['occupation'])  # Output: Engineer

# Modifying the value of an existing key
my_dict['age'] = 26
print("Updated Age:", my_dict['age'])  # Output: 26

# Checking if a key exists in the dictionary
if 'gender' in my_dict:
    print("Gender:", my_dict['gender'])
else:
    print("Gender key does not exist in the dictionary.")

# Using get() method to access a value with a default if the key is not present
gender = my_dict.get('gender', 'Not specified')
print("Gender:", gender)  # Output: Not specified

# Removing a key-value pair from the dictionary
removed_value = my_dict.pop('occupation')
print("Removed Occupation:", removed_value)  # Output: Engineer

# Iterating through keys and values
for key, value in my_dict.items():
    print(f"{key}: {value}")

# Creating a dictionary with mixed key types
mixed_dict = {'name': 'Alice', 42: 'answer', (1, 2): 'tuple'}
print(mixed_dict)

# Dictionary comprehension
squared_numbers = {x: x**2 for x in range(5)}
print(squared_numbers)

# Nested dictionaries
nested_dict = {'person': {'name': 'Bob', 'age': 30, 'city': 'London'}}
print("Nested Dictionary:", nested_dict['person']['name'])  # Output: Bob
