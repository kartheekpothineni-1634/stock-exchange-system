📘 Project Title

Stock Exchange Transaction Management System Using Doubly Linked List in C

👥 Team Members

Student 1:P.Kartheek

Student 2:N.Yaswanth



📌 Problem Statement

In a stock exchange environment, large numbers of transactions (buy/sell of stocks) are generated continuously. Managing these transactions efficiently requires dynamic data handling, fast access, and flexible operations like insertion, deletion, updating, and searching.

Traditional static data structures are not suitable because:

The number of transactions is not fixed
Memory needs to be allocated dynamically
Frequent updates are required

Objective:
To design and implement a menu-driven system in C that efficiently manages stock transactions using dynamic memory allocation and supports CRUD operations along with sorting and file storage.




🧠 Data Structures Used
1. Structure (struct Transaction)

Stores transaction details:

Transaction ID
Stock Name
Quantity
Price
Pointers (prev, next)
2. Doubly Linked List
Each node represents a transaction
Contains:
Pointer to previous node
Pointer to next node

Why used?

Efficient insertion and deletion
Traversal in both directions
Dynamic memory allocation



⚙️ Algorithm Explanation
1. Add Transaction
Create a new node using malloc
Read transaction details from user
Insert node at the end of the list
Update prev and next pointers

2. Delete Transaction
Input transaction ID
Traverse list to find node
Adjust pointers:
prev->next = next
next->prev = prev
Free memory using free()

3. Update Transaction
Search for transaction using ID
Modify fields (stock name, quantity, price)

4. Search Transaction
Traverse list
Compare ID
Display transaction if found

5. Display Transactions
Traverse from head to end
Print all node values

6. Sort Transactions (by Price)
Use nested loops
Compare prices of nodes
Swap data between nodes

7. Save to File
Open file in write mode
Traverse list
Write each transaction to file

8. Load from File
Open file in read mode
Read transaction data
Create nodes dynamically
Insert into list




🖥️ Compilation Instructions
Using GCC Compiler:
gcc stock_exchange.c -o stock_exchange
./stock_exchange
Steps:
Save code as stock_exchange.c
Open terminal / command prompt
Compile using gcc
Run executable file


<img width="528" height="653" alt="Screenshot 2026-05-04 204530" src="https://github.com/user-attachments/assets/cabcd36c-4ebf-4bfc-ae77-5b7729616a00" />
<img width="408" height="324" alt="Screenshot 2026-05-04 204543" src="https://github.com/user-attachments/assets/500af9fd-b3d0-4cba-ab5d-de9cdceca294" />
<img width="363" height="280" alt="Screenshot 2026-05-04 204559" src="https://github.com/user-attachments/assets/3598f2f1-035d-4e69-a023-4fb994d5ca39" />
<img width="430" height="324" alt="Screenshot 2026-05-04 204611" src="https://github.com/user-attachments/assets/7cf9d862-11ca-4303-895e-90c41f09b7ca" />
<img width="441" height="275" alt="Screenshot 2026-05-04 204619" src="https://github.com/user-attachments/assets/6c352bda-a175-495b-a25f-b9a3e453f0bd" />
<img width="433" height="307" alt="Screenshot 2026-05-04 204628" src="https://github.com/user-attachments/assets/4f841cf8-ecf8-4812-8ad7-5acdfd7bf8a7" />
<img width="399" height="319" alt="Screenshot 2026-05-04 204638" src="https://github.com/user-attachments/assets/64a101b6-499d-465f-bed4-af50aba83450" />
<img width="427" height="251" alt="Screenshot 2026-05-04 204646" src="https://github.com/user-attachments/assets/591a6963-aeb9-4ed3-b1e6-8df01ab608ce" />
<img width="456" height="259" alt="Screenshot 2026-05-04 204656" src="https://github.com/user-attachments/assets/abd132c2-c976-4ecf-b966-117a2714c163" />
<img width="438" height="257" alt="Screenshot 2026-05-04 204705" src="https://github.com/user-attachments/assets/4dc00cc5-cd95-42ef-ac58-84fdcc3c521a" />
<img width="373" height="241" alt="Screenshot 2026-05-04 204713" src="https://github.com/user-attachments/assets/c19c1639-5124-45fe-8a0e-1f2e1dad0b3c" />







📂 Files Used
1. Source File
stock_exchange.c → Contains full program
2. Data File
transactions.txt → Stores transaction records permanently




✨ Features of the System
✔ Menu-driven interface
✔ Dynamic memory allocation (malloc, free)
✔ Doubly linked list implementation
✔ CRUD operations:
Create (Add)
Read (Display/Search)
Update
Delete
✔ Sorting transactions by price
✔ Forward and reverse traversal
✔ File handling (save & load data)
✔ Memory management (no leaks)



🧾 Conclusion

The Stock Exchange Transaction Management System successfully demonstrates the use of dynamic data structures in C. By using a doubly linked list, the system efficiently handles real-time transaction operations such as insertion, deletion, updating, and searching.

The addition of file handling enhances the system by providing data persistence, making it more practical and closer to real-world applications. This project highlights the importance of proper memory management and modular programming in developing scalable systems
