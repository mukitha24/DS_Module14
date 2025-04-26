# Ex.No(2A) Dequeue Elements from Circular Queue
## DATE:03-03-25
## AIM:
To write a C program to delete three elements from the filled circular queue.

## Algorithm
1. Start
2. Define a queue with a fixed size SIZE and initialize front and rear pointers.
3. Define the deQueue() function to remove and return an element from the front of the queue.
4. Check if the queue is empty using isEmpty(); if empty, print an error message.
5. If the queue has one element, reset both front and rear to -1.
6. If the queue has more than one element, update front to the next index using modulo
operation ((front + 1) % SIZE).
7. Return the removed element from the front of the queue.
8. End

## Program:
```
/*
Program to delete three elements from the filled circular queue
Developed by: MUKITHA V M
RegisterNumber: 212223040119 
*/
```
```
/*#include<stdio.h>
#define SIZE 5
int items[SIZE];
int front =-1,rear =-1;
*/
int deQueue()
{
int element;
element=items[front];
if(isEmpty())
{
printf("Queue isEmpty!!");
}
else
{
if(front==rear)
{
front=-1;
rear=-1;
}
else
{
front=(front+1)%SIZE;
}
}
return element;
}
```
## Output:
![Screenshot 2025-04-26 160014](https://github.com/user-attachments/assets/f4a9d3f5-9860-470b-965e-9696fd61a5d5)
## Result:
Thus, the C program to delete three elements from the filled circular queue is implemented successfully.
