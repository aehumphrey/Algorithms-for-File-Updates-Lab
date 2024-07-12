# Algorithms for File Updates Lab

## Objective

In this scenario, access to restricted content is controlled via IP address. The “allow_list.txt” file contains these IP addresses. A separate remove list identifies IP addresses that should no longer have authorization. I created an algorithm in Python to automate updating the “allow_list.txt file.”

### Skills Learned

- Proficiency in file handling operations such as opening, reading, writing, and closing files using Python's built-in functions.
- Competence in manipulating strings and text data extracted from .txt files.
- Ability to design and optimize algorithms for efficient updating of .txt files, particularly when handling large volumes of data.
- Skill in documenting code effectively through comments and docstrings for readability and maintenance purposes.
- Understanding of different file formats and parsing techniques, depending on the structure and content of the .txt file being updated.
- Application of Python programming skills to practical scenarios involving file manipulation and data processing tasks.

## Steps

### Step One

Description: Open the file that contains the allow list

First, I opened the **“allow_list.txt” **file and assigned the file name as a string to the **import_file** variable. I also created the list **remove_list** with a list of IP addresses that should not be authorized to access the restricted information:

![image](https://github.com/user-attachments/assets/daaf449e-dbb2-40f7-95ab-d7e8cfbf6251)

_Ref 1: Creating allow_list and remove_list_

Next, I used a with statement to open the file:

![image](https://github.com/user-attachments/assets/c4a9413a-abf1-412e-84ca-1946442082b6)

_Ref 2: Opening the file using a with statement._

In order to access the IP addresses stored in the allow file, I need to first open the file. The **with** keyword manages resources by closing the file after exiting the with statement. The **open()** function in this code has two parameters: first, identifying the file to import (in this case, **import_file**); the second, what I want to do with this file (in this case, **“r”**, meaning read). I’ve also used the **as** keyword to assign a variable named **file** to store the output of the **.open()** function. 


### Step Two

Description: Read the file contents

When using an **.open()** function that includes the argument **”r”,** I can call the **.read()** function in the body of the **with** statement. This converts the file into a string format, allowing me to read it and, later, to use the string to organize and extract data. I assigned the string output of **file.read()** to the variable **ip_addresses**:

![image](https://github.com/user-attachments/assets/d9b9648e-2028-46a5-8852-0dc19231598a)

_Ref 3. Using the file.read() function to read a .txt file_

Below is the output of the function:

![image](https://github.com/user-attachments/assets/c4cf6ecb-e3a1-4b27-b41d-dd093db61c14)

_Ref 4. Output of file.read()_




### Step Three

Description: Convert the string into a list

### Step Four

Description: Iterate through the remove list

### Step Five

Description: Remove IP addresses that are on the remove list

### Step Six

Description: Update the file with the revised list of IP addresses 



