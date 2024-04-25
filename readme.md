# Python Codes?!

- Basic
    - Check Prime
        
        ```python
        def is_prime(num):
            if num < 2:
                return False
            for i in range(2, int(num**0.5) + 1):
                if num % i == 0:
                    return False
            return True
        
        # Print prime numbers between 1 and 100
        print("Prime numbers between 1 and 100:")
        for i in range(1, 101):
            if is_prime(i):
                print(i, end=" ")
        ```
        
    - Shuffle using random
        
        ```python
        import random
        
        # Define a list
        my_list = [1, 2, 3, 4, 5]
        
        # Shuffle the list
        random.shuffle(my_list)
        
        # Print the shuffled list
        print("Shuffled list:", my_list)
        ```
        
    - Area of Triangle
        
        ```python
        base = float(input("Enter the base of the triangle: "))
        height = float(input("Enter the height of the triangle: "))
        
        # Calculate the area of the triangle
        area = 0.5 * base * height
        
        # Print the area of the triangle
        print("The area of the triangle with base", base, "and height", height, "is:", area
        ```
        
    - Write a program to implement Employee class.
        
        ```python
        class Employee:
            def __init__(self, name, age, department):
                self.name = name
                self.age = age
                self.department = department
        
            def display_info(self):
                print("Name:", self.name)
                print("Age:", self.age)
                print("Department:", self.department)
        
        # Create an instance of Employee class
        emp1 = Employee("John Doe", 30, "Engineering")
        
        # Display information about the employee
        emp1.display_info()
        
        ```
        
    - Write a program to implement constructors.
        
        ```python
        class Student:
            def __init__(self, name, age, grade):
                self.name = name
                self.age = age
                self.grade = grade
        
            def display_info(self):
                print("Name:", self.name)
                print("Age:", self.age)
                print("Grade:", self.grade)
        
        # Create instances of the Student class using constructors
        student1 = Student("Alice", 18, "A")
        student2 = Student("Bob", 17, "B")
        
        # Display information about the students
        print("Information about Student 1:")
        student1.display_info()
        print("\nInformation about Student 2:")
        student2.display_info()
        
        ```
        
    - Create file in different modes
        
        ```python
        # Create a file in write mode ('w')
        with open('file_write.txt', 'w') as file:
            file.write("This is a test file created in write mode.")
        
        # Create a file in append mode ('a')
        with open('file_append.txt', 'a') as file:
            file.write("\nThis is a test file created in append mode.")
        
        # Create a file in write binary mode ('wb')
        with open('file_write_binary.txt', 'wb') as file:
            file.write(b"This is a test file created in write binary mode.")
        
        # Create a file in read mode ('r') - This will create a new file only if it does not exist
        with open('file_read.txt', 'r') as file:
            content = file.read()
            print("Content of file_read.txt:", content)
        
        ```
        
- Pyramids
    - Alphabet Pyramid
        
        ```python
        rows = int(input("Enter the no. of rows : "))
        start_char = 'A'
        for i in range(rows):
            # Print characters in increasing order
            for j in range(i + 1):
                print(start_char, end=" ")
                start_char = chr(ord(start_char) + 1)  # Move to the next character
            print()  # Move to the next line
        ```
        
    - Left Star
        
        ```python
        rows = int(input("Enter the number of rows: "))
        for i in range(rows):
            print("* " * (i + 1))
        ```
        
    - Number Pyramid
        
        ```python
        rows = int(input("Enter the number of rows: 2"))
        num = 1
        
        for i in range(rows):
            # Print numbers in increasing order
            for j in range(i + 1):
                print(num, end=" ")
                num += 1
            
            print()  # Move to the next line
        ```
        
- Lists
    - Adding of Lists
        
        ```python
        def add_lists(list1, list2):
            return list1 + list2
        
        # Example lists
        list1 = [1, 2, 3]
        list2 = [4, 5, 6]
        
        # Add list1 to list2
        result_list = add_lists(list1, list2)
        
        print("List 1:", list1)
        print("List 2:", list2)
        print("Result after adding List 1 to List 2:", result_list)
        ```
        
    - Check Empty List
        
        ```python
        def check_empty_list(lst):
            if not lst:
                return True  # List is empty
            else:
                return False  # List is not empty
        
        # Example lists
        empty_list = []
        non_empty_list = [1, 2, 3]
        
        # Check if the lists are empty
        if check_empty_list(empty_list):
            print("The list is empty.")
        else:
            print("The list is not empty.")
        
        if check_empty_list(non_empty_list):
            print("The list is empty.")
        else:
            print("The list is not empty.")
        ```
        
    - To find Second Smallest Number in List
        
        ```python
        def second_smallest(numbers):
            unique_numbers = list(set(numbers))
            unique_numbers.sort()
            return unique_numbers[1] if len(unique_numbers) > 1 else None
        my_list = [4, 10, 1, 3, 4, 2, 1]
        print("Second smallest:", second_smallest(my_list))
        ```
        
    - To find Smallest Number in List
        
        ```python
        def find_smallest_number(lst):
            if not lst:
                return None  # Return None if the list is empty
            else:
                return min(lst)
        
        # Example list
        my_list = [10, 5, 8, 3, 12, 7]
        
        # Find the smallest number in the list
        smallest_number = find_smallest_number(my_list)
        
        if smallest_number is not None:
            print("The smallest number in the list is:", smallest_number)
        else:
            print("The list is empty.")
        ```
        
    - Swapping First and Last Number
        
        ```python
        def swap_first_last(lst):
            if len(lst) > 1:
                lst[0], lst[-1] = lst[-1], lst[0]
            return lst
        
        # Example usage:
        my_list = [4, 10, 1, 3, 4, 2, 1]
        print("Swapped list:", swap_first_last(my_list))
        ```
        
    - Unique Values
        
        ```python
        def unique_values(my_list):
            return list(set(my_list))
        
        my_list = [4, 10, 1, 3, 4, 2, 1]
        print("Unique:", unique_values(my_list))
        ```
        
- Dictionary
    - Ascending and Descending order
        
        ```python
        # Dictionary to be sorted
        my_dict = {'a': 5, 'b': 2, 'c': 7, 'd': 1, 'e': 9}
        
        # Sorting dictionary by values in ascending order
        sorted_dict_asc = {k: v for k, v in sorted(my_dict.items(), key=lambda item: item[1])}
        
        print("Dictionary sorted by values in ascending order:")
        print(sorted_dict_asc)
        
        # Sorting dictionary by values in descending order
        sorted_dict_desc = {k: v for k, v in sorted(my_dict.items(), key=lambda item: item[1], reverse=True)}
        
        print("\nDictionary sorted by values in descending order:")
        print(sorted_dict_desc)
        ```
        
    - Write a program in python to map 2 lists into a dictionary.
        
        ```python
        # Define two lists
        keys = ['a', 'b', 'c']
        values = [1, 2, 3]
        
        # Map two lists into a dictionary
        dictionary = dict(zip(keys, values))
        
        # Print the dictionary
        print("Dictionary:", dictionary)
        
        ```
        
    - Write a program to concatenate two dictionaries to create one
        
        ```python
        # Define two dictionaries
        dict1 = {'a': 1, 'b': 2}
        dict2 = {'c': 3, 'd': 4}
        
        # Concatenate the dictionaries
        concat_dict = {**dict1, **dict2}
        
        # Print the concatenated dictionary
        print("Concatenated dictionary:", concat_dict)
        
        ```
        
    - Write a program to make dictionary of list of ‘n’ students.
        
        ```python
        def create_student_dictionary(n):
            student_dict = {}
            for i in range(1, n+1):
                name = input(f"Enter name of student {i}: ")
                age = int(input(f"Enter age of student {i}: "))
                grade = input(f"Enter grade of student {i}: ")
                
                student_info = {'Name': name, 'Age': age, 'Grade': grade}
                student_dict[f'Student {i}'] = student_info
            
            return student_dict
        
        # Input the number of students
        num_students = int(input("Enter the number of students: "))
        
        # Create the dictionary of lists for 'n' students
        student_dictionary = create_student_dictionary(num_students)
        
        # Print the student dictionary
        print("\nStudent Dictionary:")
        for student, info in student_dictionary.items():
            print(student, ":", info)
        
        ```
        
    - Write a Python program to print all distinct values in a dictionary.
        
        ```python
        def print_distinct_values(my_dict):
            distinct_values = set(my_dict.values())
            for value in distinct_values:
                print(value)
        
        # Example dictionary
        my_dict = {'a': 1, 'b': 2, 'c': 1, 'd': 3, 'e': 2}
        
        # Print distinct values
        print_distinct_values(my_dict)
        
        ```
        
- String
    - Write a Python program to calculate the length of a string
        
        ```python
        def string_length(str1):
            count = 0
            for char in str1:
                count += 1
            return count
        
        print(string_length("Python Programming"))
        
        ```
        
    - Write a Python function that takes a list of words and return the longest word and the length of the longest one
        
        ```python
        def find_longest_word(word_list):
            longest_word = max(word_list, key=len)
            return longest_word, len(longest_word)
        
        # Example usage:
        words = ["Python", "Programming", "Code", "Browser", "Function"]
        longest_word, length = find_longest_word(words)
        
        print("Longest word:", longest_word)
        print("Length of the longest word:", length)
        
        ```
        
    - Append new string in the middle of a given string
        
        ```python
        def insert_string_middle(str, word):
            return str[:len(str)//2] + word + str[len(str)//2:]
        
        print(insert_string_middle('[[]]', 'Python'))
        
        ```
        
    - Write a Python program to count the number of characters (character frequency) in a string.
        
        ```python
        def char_frequency(str1):
            dict = {}
            for n in str1:
                keys = dict.keys()
                if n in keys:
                    dict[n] += 1
                else:
                    dict[n] = 1
            return dict
        
        print(char_frequency("Python Programming"))
        
        ```
        
- Tuple
    - Swap two tuples in Python
        
        ```python
        # Define two tuples
        tup1 = (1, 2, 3)
        tup2 = (4, 5, 6)
        
        # Swap the tuples
        tup1, tup2 = tup2, tup1
        
        # Print the swapped tuples
        print("Tuple 1:", tup1)
        print("Tuple 2:", tup2)
        
        ```
        
    - Write a Python program to create a tuple with different data types
        
        ```python
        # create a tuple with different data types
        tuplex = ("tuple", False, 3.2, 1)
        print(tuplex)
        
        ```
        
    - Write a Python program to get the 4th element from the last
    element of a tuple
        
        ```python
        # Define a tuple
        my_tuple = (10, 20, 30, 40, 50, 60)
        
        # Get the 4th element from the last
        fourth_from_last = my_tuple[-4]
        
        # Print the result
        print("The 4th element from the last of the tuple is:", fourth_from_last)
        
        ```
        
    - Write a Python program to convert a tuple to a string.
        
        ```python
        # Define a tuple
        my_tuple = (10, 20, 30, 40, 50)
        
        # Convert tuple to string
        tuple_string = ''.join(map(str, my_tuple))
        
        # Print the result
        print("Tuple converted to string:", tuple_string)
        
        ```
        
    - Check Element
        
        ```python
        # Define a tuple
        my_tuple = (10, 20, 30, 40, 50)
        
        # Element to check
        element_to_check = 30
        
        # Check if element exists in tuple
        if element_to_check in my_tuple:
            print("Element", element_to_check, "exists in the tuple.")
        else:
            print("Element", element_to_check, "does not exist in the tuple.")
        
        ```
        
    - Swap 2 Tuples
        
        ```python
        # Original tuples
        tuple1 = (1, 2, 3)
        tuple2 = (4, 5, 6)
        
        # Print original tuples
        print("Original tuple1:", tuple1)
        print("Original tuple2:", tuple2)
        
        # Swapping
        tuple1, tuple2 = tuple2, tuple1
        
        # Print swapped tuples
        print("Swapped tuple1:", tuple1)
        print("Swapped tuple2:", tuple2)
        
        ```
        
- Numpy Array
    - Create a 1D array of numbers from 0 to 9
        
        ```python
        import numpy as np
        
        # Create a 1D array of numbers from 0 to 9
        arr = np.arange(10)
        
        print("1D Array:", arr)
        
        ```
        
    - Create a 3×3 numpy array of all True’s
        
        ```python
        import numpy as np
        
        # Create a 3x3 numpy array of all True's
        arr = np.full((3, 3), True, dtype=bool)
        
        print("3x3 Array of True's:")
        print(arr)
        
        ```
        
    - Create a 3x3 identity matrix
        
        ```python
        import numpy as np
        
        # Create a 3x3 identity matrix
        identity_matrix = np.eye(3)
        
        print("3x3 Identity Matrix:")
        print(identity_matrix)
        
        ```
        
    - Extract all odd numbers from array.
        
        ```python
        import numpy as np
        
        # Create an array
        arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9])
        
        # Extract odd numbers
        odd_numbers = arr[arr % 2 != 0]
        
        print("Odd Numbers in the Array:", odd_numbers)
        
        ```
        
    - Replace all odd numbers in array with -1
        
        ```python
        import numpy as np
        
        # Create an array
        arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9])
        
        # Replace odd numbers with -1
        arr[arr % 2 != 0] = -1
        
        print("Array with odd numbers replaced by -1:", arr)
        
        ```
        
    - Replace all odd numbers in arr with -1 without changing arr
        
        ```python
        import numpy as np
        
        # Original array
        arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9])
        
        # Create a copy of the original array
        new_arr = np.copy(arr)
        
        # Replace odd numbers in the copy with -1
        new_arr[new_arr % 2 != 0] = -1
        
        # Print the original and modified arrays
        print("Original array:", arr)
        print("Array with odd numbers replaced by -1:", new_arr)
        
        ```
        
    - Stack arrays a and b vertically
        
        ```python
        import numpy as np
        
        # Example arrays a and b
        a = np.array([[1, 2, 3],
                      [4, 5, 6]])
        
        b = np.array([[7, 8, 9],
                      [10, 11, 12]])
        
        # Stack arrays vertically
        stacked_array = np.vstack((a, b))
        
        print("Stacked array:")
        print(stacked_array)
        
        ```
        
    - From array a remove all items present in array b
        
        ```python
        import numpy as np
        
        # Example arrays a and b
        a = np.array([1, 2, 3, 4, 5])
        b = np.array([3, 4, 7, 8])
        
        # Remove items present in array b from array a
        result = np.setdiff1d(a, b)
        
        print("Result array after removing items present in b from a:")
        print(result)
        
        ```
        
    - Get the positions where elements of a and b match(a and b are arrays)
        
        ```python
        import numpy as np
        
        # Example arrays a and b
        a = np.array([1, 2, 3, 4, 5])
        b = np.array([3, 4, 7, 8, 2])
        
        # Get the positions where elements of a and b match
        matches = np.where(a == b)
        
        print("Positions where elements of a and b match:")
        print(matches)
        
        ```
        
    - Get all items between 5 and 10 from array
        
        ```python
        import numpy as np
        
        # Example array
        arr = np.array([2, 4, 6, 8, 10, 12, 14, 16])
        
        # Get all items between 5 and 10
        result = arr[(arr >= 5) & (arr <= 10)]
        
        print("Items between 5 and 10:", result)
        
        ```
        
    - Reverse the rows of a 2D array arr.
        
        ```python
        import numpy as np
        
        # Example 2D array
        arr = np.array([[1, 2, 3],
                        [4, 5, 6],
                        [7, 8, 9]])
        
        # Reverse the rows of the array
        reversed_arr = arr[::-1]
        
        print("Original array:")
        print(arr)
        
        print("\nArray with reversed rows:")
        print(reversed_arr)
        
        ```
        
    - Create a 2D array of shape 5x3 to contain random decimal numbers between 5 and 10.
        
        ```python
        import numpy as np
        
        # Create a 2D array of shape 5x3 with random decimal numbers between 5 and 10
        random_array = np.random.uniform(5, 10, size=(5, 3))
        
        print("2D Array of random decimal numbers between 5 and 10:")
        print(random_array)
        ```
        
    - Limit the number of items printed in python numpy array a to a maximum of 6 elements.
        
        ```python
        import numpy as np
        
        # Example array
        a = np.arange(10)
        
        # Set the maximum number of items to be displayed
        np.set_printoptions(threshold=6)
        
        print("Array a with a maximum of 6 elements displayed:")
        print(a)
        
        ```
        
- Lambda Functions
    - Write a Python program to create a function that takes one argument, and that argument will be multiplied with an unknown given number.
        
        ```python
        def multiply_with_unknown(x):
            # Define the unknown given number
            unknown_number = 10
            
            # Multiply the argument with the unknown given number
            result = x * unknown_number
            
            # Return the result
            return result
        
        # Example usage of the function
        argument = 5
        result = multiply_with_unknown(argument)
        print("Result of multiplying", argument, "with an unknown given number:", result)
        
        ```
        
    - Find whether a given string starts with a given character using Lambda
        
        ```python
        starts_with_char = lambda string, char: string.startswith(char)
        
        # Example usage
        given_string = "hello"
        given_char = "h"
        
        # Check if the given string starts with the given character
        result = starts_with_char(given_string, given_char)
        
        # Print the result
        print("Does the string start with the character?", result)
        
        ```
        
    - Write a Python program that multiplies each number in a list with a given number using lambda functions.
        
        ```python
        # Define a list of numbers
        numbers = [1, 2, 3, 4, 5]
        
        # Define the given number
        given_number = 10
        
        # Use lambda function to multiply each number in the list with the given number
        result = list(map(lambda x: x * given_number, numbers))
        
        # Print the result
        print("Result after multiplying each number with", given_number, ":", result)
        
        ```
        
    - Write a Python program to find the intersection of two given arrays using Lambda.
        
        ```python
        # Define two given arrays
        array1 = [1, 2, 3, 4, 5]
        array2 = [4, 5, 6, 7, 8]
        
        # Use a lambda function with filter to find the intersection
        intersection = list(filter(lambda x: x in array1, array2))
        
        # Print the intersection
        print("Intersection of the two arrays:", intersection)
        
        ```
        
    - Write a Python program to count the even and odd numbers in a given array of integers using Lambda.
        
        ```python
        # Define the given array of integers
        array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
        
        # Use lambda functions with filter to count even and odd numbers
        even_count = len(list(filter(lambda x: x % 2 == 0, array)))
        odd_count = len(list(filter(lambda x: x % 2 != 0, array)))
        
        # Print the counts
        print("Count of even numbers:", even_count)
        print("Count of odd numbers:", odd_count)
        
        ```
        
    - Write a Python program that multiplies each number in a list with a givennumber using lambda functions.
        
        ```python
        # Define the list of numbers
        numbers = [1, 2, 3, 4, 5]
        
        # Define the given number
        given_number = 10
        
        # Use lambda function with map to multiply each number in the list with the given number
        result = list(map(lambda x: x * given_number, numbers))
        
        # Print the result
        print("Result after multiplying each number with", given_number, ":", result)
        
        ```
        
    - Write a Python program to count the even and odd numbers in a given array of integers using Lambda.
        
        ```python
        # Define the given array of integers
        array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
        
        # Use lambda functions with filter to count even and odd numbers
        even_count = len(list(filter(lambda x: x % 2 == 0, array)))
        odd_count = len(list(filter(lambda x: x % 2 != 0, array)))
        
        # Print the counts
        print("Count of even numbers:", even_count)
        print("Count of odd numbers:", odd_count)
        
        ```
        
- Built In Functions
    - Write a program which contains list, tuple, dictionary using built-in methods
        
        ```python
        # List
        my_list = [1, 2, 3, 4, 5]
        
        # Tuple
        my_tuple = (6, 7, 8, 9, 10)
        
        # Dictionary
        my_dict = {'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5}
        
        # List built-in methods
        print("List built-in methods:")
        print("Length of list:", len(my_list))
        print("Index of element 3 in list:", my_list.index(3))  # Index of element
        my_list.append(6)  # Append element to list
        print("After appending 6 to list:", my_list)
        
        # Tuple built-in methods
        print("\nTuple built-in methods:")
        print("Length of tuple:", len(my_tuple))
        print("Index of element 8 in tuple:", my_tuple.index(8))  # Index of element
        
        # Dictionary built-in methods
        print("\nDictionary built-in methods:")
        print("Length of dictionary:", len(my_dict))
        print("Keys in dictionary:", my_dict.keys())
        print("Values in dictionary:", my_dict.values())
        
        ```
        
    - Write a program to understand Built-in Set and String functions
        
        ```python
        # Built-in Set functions
        print("Built-in Set functions:")
        # Creating sets
        set1 = {1, 2, 3, 4, 5}
        set2 = {4, 5, 6, 7, 8}
        
        # Union of sets
        print("Union of sets:", set1.union(set2))
        
        # Built-in String functions
        print("\nBuilt-in String functions:")
        # String methods
        string = "Hello, World!"
        print("Original String:", string)
        
        # Convert to lowercase
        print("Lowercase:", string.lower())
        
        # Split the string into a list of substrings
        print("Split string:", string.split(","))
        
        ```
        
- User-Defined and Menu Driven
    - Create User-defined modules/packages and import them in a program
        
        math.py
        
        ```python
        # math_operations.py
        
        def add(x, y):
            return x + y
        
        def subtract(x, y):
            return x - y
        
        def multiply(x, y):
            return x * y
        
        def divide(x, y):
            if y == 0:
                return "Cannot divide by zero"
            return x / y
        
        ```
        
        main.py
        
        ```python
        # main_program.py
        
        import math_operations
        
        # Test the functions from the math_operations module
        print("Addition:", math_operations.add(5, 3))
        print("Subtraction:", math_operations.subtract(5, 3))
        print("Multiplication:", math_operations.multiply(5, 3))
        print("Division:", math_operations.divide(5, 3))
        
        ```
        
    - Create user defined multithreaded application with thread synchronization and deadlocks
        
        ```python
        import threading
        import time
        
        # Define a global lock
        lock1 = threading.Lock()
        lock2 = threading.Lock()
        
        # Function to perform task 1
        def task1():
            print("Thread 1: Acquiring lock 1")
            with lock1:
                print("Thread 1: Lock 1 acquired")
                time.sleep(1)
                print("Thread 1: Acquiring lock 2")
                with lock2:
                    print("Thread 1: Lock 2 acquired")
                    # Perform task 1
                    print("Thread 1: Performing task 1")
                    time.sleep(1)
            print("Thread 1: Releasing locks")
            lock1.release()
            lock2.release()
        
        # Function to perform task 2
        def task2():
            print("Thread 2: Acquiring lock 2")
            with lock2:
                print("Thread 2: Lock 2 acquired")
                time.sleep(1)
                print("Thread 2: Acquiring lock 1")
                with lock1:
                    print("Thread 2: Lock 1 acquired")
                    # Perform task 2
                    print("Thread 2: Performing task 2")
                    time.sleep(1)
            print("Thread 2: Releasing locks")
            lock1.release()
            lock2.release()
        
        # Create threads
        thread1 = threading.Thread(target=task1)
        thread2 = threading.Thread(target=task2)
        
        # Start threads
        thread1.start()
        thread2.start()
        
        # Join threads
        thread1.join()
        thread2.join()
        
        print("Multithreaded application completed")
        
        ```
        
    - Create a menu driven application which should cover all the built-in exceptions in python
        
        ```python
        def divide(x, y):
            try:
                result = x / y
                print("Result of division:", result)
            except ZeroDivisionError:
                print("Error: Division by zero!")
            except TypeError:
                print("Error: Unsupported operand type(s) for division!")
            except Exception as e:
                print("An unexpected error occurred:", e)
        
        def access_list_element(lst, index):
            try:
                value = lst[index]
                print("Value at index", index, ":", value)
            except IndexError:
                print("Error: Index out of range!")
            except Exception as e:
                print("An unexpected error occurred:", e)
        
        def open_file(filename):
            try:
                with open(filename, 'r') as file:
                    content = file.read()
                    print("Content of file:")
                    print(content)
            except FileNotFoundError:
                print("Error: File not found!")
            except PermissionError:
                print("Error: Permission denied!")
            except Exception as e:
                print("An unexpected error occurred:", e)
        
        while True:
            print("\nMenu:")
            print("1. Perform division")
            print("2. Access list element")
            print("3. Open file")
            print("4. Exit")
        
            choice = input("Enter your choice (1/2/3/4): ")
        
            if choice == '1':
                x = float(input("Enter numerator: "))
                y = float(input("Enter denominator: "))
                divide(x, y)
            elif choice == '2':
                lst = [1, 2, 3, 4, 5]
                index = int(input("Enter index: "))
                access_list_element(lst, index)
            elif choice == '3':
                filename = input("Enter filename: ")
                open_file(filename)
            elif choice == '4':
                print("Exiting the program.")
                break
            else:
                print("Invalid choice! Please enter a valid option.")
        
        ```
        
- GUI - Tkinter
    - Write python programs to design registration page using built-in tools in python (Tkinter)
        
        ```python
        import tkinter as tk
        from tkinter import messagebox
        
        def register():
            username = username_entry.get()
            password = password_entry.get()
            confirm_password = confirm_password_entry.get()
        
            if username == "" or password == "" or confirm_password == "":
                messagebox.showerror("Error", "All fields are required!")
            elif password != confirm_password:
                messagebox.showerror("Error", "Passwords do not match!")
            else:
                messagebox.showinfo("Success", "Registration successful for username: " + username)
                # You can save the username and password to a file or database here
        
        # Create the main window
        root = tk.Tk()
        root.title("Registration Page")
        
        # Create labels
        username_label = tk.Label(root, text="Username:")
        username_label.grid(row=0, column=0, padx=10, pady=5)
        password_label = tk.Label(root, text="Password:")
        password_label.grid(row=1, column=0, padx=10, pady=5)
        confirm_password_label = tk.Label(root, text="Confirm Password:")
        confirm_password_label.grid(row=2, column=0, padx=10, pady=5)
        
        # Create entry widgets
        username_entry = tk.Entry(root)
        username_entry.grid(row=0, column=1, padx=10, pady=5)
        password_entry = tk.Entry(root, show="*")
        password_entry.grid(row=1, column=1, padx=10, pady=5)
        confirm_password_entry = tk.Entry(root, show="*")
        confirm_password_entry.grid(row=2, column=1, padx=10, pady=5)
        
        # Create register button
        register_button = tk.Button(root, text="Register", command=register)
        register_button.grid(row=3, column=0, columnspan=2, padx=10, pady=10)
        
        # Run the application
        root.mainloop()
        
        ```
        
    - Write python programs to design calculator page using built-in tools in python
        
        ```python
        import tkinter as tk
        from tkinter import messagebox
        
        def calculate():
            try:
                expression = entry.get()
                result = eval(expression)
                entry.delete(0, tk.END)
                entry.insert(tk.END, str(result))
            except Exception as e:
                messagebox.showerror("Error", "Invalid input!")
        
        def clear():
            entry.delete(0, tk.END)
        
        def add_to_entry(char):
            entry.insert(tk.END, char)
        
        # Create the main window
        root = tk.Tk()
        root.title("Calculator")
        
        # Create the entry widget
        entry = tk.Entry(root, width=30, borderwidth=5)
        entry.grid(row=0, column=0, columnspan=4, padx=10, pady=10)
        
        # Create buttons for numbers and operators
        buttons = [
            ('7', 1, 0), ('8', 1, 1), ('9', 1, 2), ('/', 1, 3),
            ('4', 2, 0), ('5', 2, 1), ('6', 2, 2), ('*', 2, 3),
            ('1', 3, 0), ('2', 3, 1), ('3', 3, 2), ('-', 3, 3),
            ('0', 4, 0), ('.', 4, 1), ('=', 4, 2), ('+', 4, 3)
        ]
        
        for (text, row, column) in buttons:
            button = tk.Button(root, text=text, padx=20, pady=10, command=lambda char=text: add_to_entry(char))
            button.grid(row=row, column=column, padx=5, pady=5)
        
        # Clear button
        clear_button = tk.Button(root, text='Clear', padx=50, pady=10, command=clear)
        clear_button.grid(row=5, column=0, columnspan=4, padx=10, pady=10)
        
        # Run the application
        root.mainloop()
        
        ```
        
    - Write python programs to design Login page using built-in tools in python
        
        ```python
        import tkinter as tk
        from tkinter import messagebox
        
        def login():
            username = username_entry.get()
            password = password_entry.get()
        
            # You can replace the condition with actual authentication logic
            if username == "admin" and password == "password":
                messagebox.showinfo("Success", "Login successful!")
            else:
                messagebox.showerror("Error", "Invalid username or password")
        
        # Create the main window
        root = tk.Tk()
        root.title("Login Page")
        
        # Create labels
        username_label = tk.Label(root, text="Username:")
        username_label.grid(row=0, column=0, padx=10, pady=5)
        password_label = tk.Label(root, text="Password:")
        password_label.grid(row=1, column=0, padx=10, pady=5)
        
        # Create entry widgets
        username_entry = tk.Entry(root)
        username_entry.grid(row=0, column=1, padx=10, pady=5)
        password_entry = tk.Entry(root, show="*")
        password_entry.grid(row=1, column=1, padx=10, pady=5)
        
        # Create login button
        login_button = tk.Button(root, text="Login", command=login)
        login_button.grid(row=2, column=0, columnspan=2, padx=10, pady=10)
        
        # Run the application
        root.mainloop()
        
        ```
        
- Database MySQL CRUD
    - Write python programs to perform CRUD operations in python (Use any one database like  MySQL
        
        ```python
        import mysql.connector
        
        # Establish connection to MySQL database
        db = mysql.connector.connect(
            host="localhost",
            user="your_username",
            password="your_password",
            database="your_database"
        )
        
        # Create a cursor object to interact with the database
        cursor = db.cursor()
        
        def create_record(name, age, email):
            sql = "INSERT INTO users (name, age, email) VALUES (%s, %s, %s)"
            values = (name, age, email)
            cursor.execute(sql, values)
            db.commit()
            print("Record created successfully")
        
        def read_records():
            sql = "SELECT * FROM users"
            cursor.execute(sql)
            records = cursor.fetchall()
            print("Records:")
            for record in records:
                print(record)
        
        def update_record(user_id, new_age):
            sql = "UPDATE users SET age = %s WHERE id = %s"
            values = (new_age, user_id)
            cursor.execute(sql, values)
            db.commit()
            print("Record updated successfully")
        
        def delete_record(user_id):
            sql = "DELETE FROM users WHERE id = %s"
            values = (user_id,)
            cursor.execute(sql, values)
            db.commit()
            print("Record deleted successfully")
        
        # Perform CRUD operations
        create_record("John", 30, "john@example.com")
        read_records()
        update_record(1, 35)
        read_records()
        delete_record(1)
        read_records()
        
        # Close cursor and database connection
        cursor.close()
        db.close()
        
        ```
        
- Numpy and Matplolib
    - Consider any dataset and draw different types of plots using Numpy and Matplotlob
        
        ```python
        import numpy as np
        import matplotlib.pyplot as plt
        
        # Generate random data for monthly sales
        months = np.arange(1, 13)
        sales = np.random.randint(10000, 50000, size=12)
        
        # Line plot
        plt.figure(figsize=(8, 6))
        plt.plot(months, sales, marker='o', linestyle='-')
        plt.title('Monthly Sales')
        plt.xlabel('Month')
        plt.ylabel('Sales')
        plt.grid(True)
        plt.show()
        
        # Bar plot
        plt.figure(figsize=(8, 6))
        plt.bar(months, sales, color='skyblue')
        plt.title('Monthly Sales')
        plt.xlabel('Month')
        plt.ylabel('Sales')
        plt.xticks(months)
        plt.grid(axis='y')
        plt.show()
        
        # Histogram
        plt.figure(figsize=(8, 6))
        plt.hist(sales, bins=5, color='lightgreen', edgecolor='black')
        plt.title('Monthly Sales Distribution')
        plt.xlabel('Sales')
        plt.ylabel('Frequency')
        plt.grid(axis='y')
        plt.show()
        
        # Scatter plot (with random expenses data)
        expenses = np.random.randint(2000, 10000, size=12)
        plt.figure(figsize=(8, 6))
        plt.scatter(sales, expenses, color='orange', marker='o')
        plt.title('Sales vs Expenses')
        plt.xlabel('Sales')
        plt.ylabel('Expenses')
        plt.grid(True)
        plt.show()
        
        ```
        
- Pandas with DATAFRAMES
    - Generate the series of dates from 1st May, 2021 to 12th May, 2021 (both inclusive)
        
        ```python
        import pandas as pd
        
        # Generate the series of dates
        start_date = '2021-05-01'
        end_date = '2021-05-12'
        date_range = pd.date_range(start=start_date, end=end_date)
        
        # Print the series of dates
        print("Series of dates from 1st May, 2021 to 12th May, 2021:")
        for date in date_range:
            print(date.strftime('%Y-%m-%d'))
        
        ```
        
    - Apply the function, f(x) = x/2 on each and every element of a given pandas series
        
        ```python
        import pandas as pd
        
        # Create a sample Pandas Series
        data = pd.Series([10, 20, 30, 40, 50])
        
        # Define the function f(x) = x/2
        def f(x):
            return x / 2
        
        # Apply the function to each element of the Series
        result = data.apply(f)
        
        # Print the original and modified Series
        print("Original Series:")
        print(data)
        print("\nAfter applying the function f(x) = x/2:")
        print(result)
        
        ```
        
    - Given a dictionary, convert it into corresponding dataframe and display it
        
        ```python
        import pandas as pd
        
        # Sample dictionary
        data = {
            'Name': ['John', 'Alice', 'Bob'],
            'Age': [30, 25, 35],
            'City': ['New York', 'London', 'Paris']
        }
        
        # Convert the dictionary to a DataFrame
        df = pd.DataFrame(data)
        
        # Display the DataFrame
        print("DataFrame:")
        print(df)
        
        ```
        
    - Given a 2D List, convert it into corresponding dataframe and display it
        
        ```python
        import pandas as pd
        
        # Sample 2D list
        data = [
            ['John', 30, 'New York'],
            ['Alice', 25, 'London'],
            ['Bob', 35, 'Paris']
        ]
        
        # Convert the 2D list to a DataFrame
        df = pd.DataFrame(data, columns=['Name', 'Age', 'City'])
        
        # Display the DataFrame
        print("DataFrame:")
        print(df)
        
        ```
        
    - Given a CSV file, read it into a dataframe and display it
        
        ```python
        import pandas as pd
        
        # Read the CSV file into a DataFrame
        df = pd.read_csv('your_file.csv')
        
        # Display the DataFrame
        print("DataFrame:")
        print(df)
        
        ```
        
    - Given a dataframe, change the index of a dataframe from the default indexes to a particular column
        
        ```python
        import pandas as pd
        
        # Create a sample DataFrame
        data = {
            'Name': ['John', 'Alice', 'Bob'],
            'Age': [30, 25, 35],
            'City': ['New York', 'London', 'Paris']
        }
        
        df = pd.DataFrame(data)
        
        # Change the index of the DataFrame to the 'Name' column
        df.set_index('Name', inplace=True)
        
        # Display the DataFrame
        print("DataFrame with 'Name' column as index:")
        print(df)
        
        ```
        
    - Given a dataframe (say, with custom indexing), sort it by it's index
        
        ```python
        import pandas as pd
        
        # Create a sample DataFrame with custom indexing
        data = {
            'Name': ['John', 'Alice', 'Bob'],
            'Age': [30, 25, 35],
            'City': ['New York', 'London', 'Paris']
        }
        
        index = ['b', 'a', 'c']  # Custom index
        
        df = pd.DataFrame(data, index=index)
        
        # Sort the DataFrame by its index
        df_sorted = df.sort_index()
        
        # Display the sorted DataFrame
        print("Sorted DataFrame by index:")
        print(df_sorted)
        
        ```
        
    - Given a dataframe, sort it by multiple columns
        
        ```python
        import pandas as pd
        
        # Create a sample DataFrame
        data = {
            'Name': ['John', 'Alice', 'Bob', 'Alice', 'Bob'],
            'Age': [30, 25, 35, 25, 30],
            'City': ['New York', 'London', 'Paris', 'London', 'New York']
        }
        
        df = pd.DataFrame(data)
        
        # Sort the DataFrame by multiple columns
        df_sorted = df.sort_values(by=['Name', 'Age'])
        
        # Display the sorted DataFrame
        print("Sorted DataFrame by multiple columns:")
        print(df_sorted)
        
        ```
        
    - Given a dataframe, select a particular column and display it
        
        ```python
        import pandas as pd
        
        # Create a sample DataFrame
        data = {
            'Name': ['John', 'Alice', 'Bob'],
            'Age': [30, 25, 35],
            'City': ['New York', 'London', 'Paris']
        }
        
        df = pd.DataFrame(data)
        
        # Select a particular column and display it
        selected_column = df['Age']  # Using indexing
        # selected_column = df.loc[:, 'Age']  # Using loc accessor
        # selected_column = df.iloc[:, 1]  # Using iloc accessor
        
        print("Selected column 'Age':")
        print(selected_column)
        
        ```
        
    - Given a dataframe, select first 2 rows and output them
        
        ```python
        import pandas as pd
        
        # Create a sample DataFrame
        data = {
            'Name': ['John', 'Alice', 'Bob', 'Eve'],
            'Age': [30, 25, 35, 28],
            'City': ['New York', 'London', 'Paris', 'Tokyo']
        }
        
        df = pd.DataFrame(data)
        
        # Select first 2 rows and output them
        first_2_rows = df.head(2)
        
        print("First 2 rows of the DataFrame:")
        print(first_2_rows)
        
        ```
        
    - Given a dataframe, select rows based on a condition
        
        ```python
        import pandas as pd
        
        # Create a sample DataFrame
        data = {
            'Name': ['John', 'Alice', 'Bob', 'Eve'],
            'Age': [30, 25, 35, 28],
            'City': ['New York', 'London', 'Paris', 'Tokyo']
        }
        
        df = pd.DataFrame(data)
        
        # Select rows where Age is greater than 25
        selected_rows = df[df['Age'] > 25]
        
        print("Rows where Age is greater than 25:")
        print(selected_rows)
        
        ```
        
    - Given is a dataframe showing name, occupation, salary of people. Find the average salary per occupation
        
        ```python
        import pandas as pd
        
        # Create a sample DataFrame
        data = {
            'Name': ['John', 'Alice', 'Bob', 'Eve', 'Mike'],
            'Occupation': ['Engineer', 'Doctor', 'Engineer', 'Teacher', 'Doctor'],
            'Salary': [50000, 60000, 55000, 45000, 65000]
        }
        
        df = pd.DataFrame(data)
        
        # Calculate average salary per occupation
        average_salary_per_occupation = df.groupby('Occupation')['Salary'].mean()
        
        print("Average salary per occupation:")
        print(average_salary_per_occupation)
        
        ```
        
    - Given a dataframe with NaN Values, fill the NaN values with 0
        
        ```python
        import pandas as pd
        import numpy as np
        
        # Create a sample DataFrame with NaN values
        data = {
            'Name': ['John', 'Alice', 'Bob', 'Eve'],
            'Occupation': ['Engineer', np.nan, 'Doctor', 'Teacher'],
            'Salary': [50000, np.nan, 55000, np.nan]
        }
        
        df = pd.DataFrame(data)
        
        # Fill NaN values with 0
        df_filled = df.fillna(0)
        
        print("DataFrame with NaN values filled with 0:")
        print(df_filled)
        
        ```
        
    - Given is a dataframe showing Company Names (cname) and corresponding Profits (profit). Convert the values of Profit column such that values in it greater than 0 are set to True and the rest are set to False.
        
        ```python
        import pandas as pd
        
        # Create a sample DataFrame
        data = {
            'cname': ['Company A', 'Company B', 'Company C', 'Company D'],
            'profit': [10000, -5000, 0, 20000]
        }
        
        df = pd.DataFrame(data)
        
        # Convert values in Profit column based on condition
        df['profit'] = df['profit'].apply(lambda x: True if x > 0 else False)
        
        print("DataFrame with Profit column values converted:")
        print(df)
        
        ```
        
    - Given a dataframe, generate the statistical summary of all the numerical features present in it
        
        ```python
        import pandas as pd
        
        # Create a sample DataFrame
        data = {
            'Name': ['John', 'Alice', 'Bob', 'Eve'],
            'Age': [30, 25, 35, 28],
            'Salary': [50000, 60000, 55000, 45000],
            'Experience': [5, 3, 7, 4]
        }
        
        df = pd.DataFrame(data)
        
        # Generate statistical summary of numerical features
        summary = df.describe()
        
        print("Statistical summary of numerical features:")
        print(summary)
        
        ```
        
    - Given are 2 dataframes, with one dataframe containing Employee ID (eid), Employee Name (ename) and Stipend (stipend) and the other dataframe containing Employee ID (eid) and designation of the employee (designation). Output the Dataframe containing Employee ID (eid), Employee Name (ename), Stipend (stipend) and Position (position).
        
        ```python
        import pandas as pd
        
        # Sample dataframes
        data1 = {
            'eid': [101, 102, 103, 104],
            'ename': ['John', 'Alice', 'Bob', 'Eve'],
            'stipend': [50000, 60000, 55000, 45000]
        }
        
        data2 = {
            'eid': [101, 102, 104, 105],
            'designation': ['Engineer', 'Doctor', 'Teacher', 'Manager']
        }
        
        df1 = pd.DataFrame(data1)
        df2 = pd.DataFrame(data2)
        
        # Merge dataframes on 'eid'
        merged_df = pd.merge(df1, df2, on='eid', how='left')
        
        # Rename the column 'designation' to 'position'
        merged_df.rename(columns={'designation': 'position'}, inplace=True)
        
        print("Merged DataFrame:")
        print(merged_df)
        
        ```
