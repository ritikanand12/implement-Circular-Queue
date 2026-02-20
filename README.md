Circular Queue Implementation in C

This project implements a Circular Queue using arrays in C programming language.

A circular queue improves the efficiency of a linear queue by reusing empty spaces created after deletions using modulo arithmetic.

📌 Description

In this program:

Queue size is fixed (N = 5)

Uses an array to store elements

Implements:

enqueue() (Insertion)

dequeue() (Deletion)

display() (Show queue elements)

Handles Overflow and Underflow conditions

🧠 What is a Circular Queue?

In a linear queue, once the rear reaches the end of the array, no more insertions are possible even if there is space at the beginning.

A Circular Queue solves this by connecting the end of the array back to the beginning using:

(rear + 1) % N

This allows efficient memory utilization.

📂 Functions Overview
🔹 enqueue(int x)

Inserts an element into the queue

Checks for overflow condition

Updates rear using modulo operation

🔹 dequeue()

Removes an element from the queue

Checks for underflow condition

Updates front accordingly

🔹 display()

Displays all elements from front to rear

▶️ Sample Execution
Operations Performed in main():
enqueue(10);
enqueue(20);
enqueue(30);
dequeue();
enqueue(40);
display();
Sample Output:
Inserted: 10
Inserted: 20
Inserted: 30
Deleted: 10
Inserted: 40
Queue: 20 30 40
⚙️ How to Compile and Run
1️⃣ Compile the program
gcc circular_queue.c -o circular_queue
2️⃣ Run the program
./circular_queue
⏱️ Time & Space Complexity

Enqueue: O(1)

Dequeue: O(1)

Display: O(N)

Space Complexity: O(N)

Where:

N = Size of the queue

📚 Concepts Covered

Queue Data Structure

Circular Queue

Modulo Arithmetic

Overflow & Underflow Handling

Array Implementation

⚠️ Limitations

Fixed size queue (static array)

Cannot dynamically resize


Dynamic circular queue using linked list

Comparison README (Linear Queue vs Circular Queue)
