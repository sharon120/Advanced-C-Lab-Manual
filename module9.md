## EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

## Aim:
To write a C program to display stack elements using an array.
## Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
## Program:
```
int top;
char stack[100];
void display()
{
    for(int i = top;i>=0;i--)
    {
        printf("%c\n",stack[i]);
    }
}
```
## Output:
![image](https://github.com/user-attachments/assets/26f848a5-7a21-4ec5-901d-c81cc1a94f59)

## Result:
Thus, the program to display stack elements using an array is verified successfully.
 

## EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
## Aim:
To create a C program to push the given element in to a stack using array.
## Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
## Program:
```
int size=3,top=-1;
float stack[100];
void push (float data)
{
    if(top==size-1)
    {
        printf("stack is full\n");
    }
    else
    {
        top++;
        stack[top]=data;
    }
}
```
## Output:
![image](https://github.com/user-attachments/assets/f38f48a5-9201-42bb-9392-087fb43fd74d)

## Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
## EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
## Aim:
To write a C program to display queue elements using array

## Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
## Program:
```
 int front = -1, rear=-1;
char queue[50];
void display()
{
    if(front ==-1||front >rear)
    {
        printf("No elements to display");
    }
    else
    {
        for(int i=front;i<=rear;i++)
        {
            printf("%c\n",queue[i]);
        }
    }
}
```
## Output:
![image](https://github.com/user-attachments/assets/38c348b6-88f9-4de4-a4ba-a5a404d99934)

## Result:
Thus, the program to display queue elements using array is verified successfully.


 
## EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
## Aim:
To write a C program to insert elements in queue using array.

## Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

## Program:
```
int front ,rear,size=3;
float queue[50];
void enqueue(float data)
{
    if(rear<=size)
    {
        if(front==-1)
        {
            front=0;
        }
        rear++;
        queue[rear]=data;
    }
}
```

## Output:
![image](https://github.com/user-attachments/assets/7d394087-b42a-4606-b2ea-9d2c5bbb7270)

## Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
## EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



## Aim:

To create a function in C that deletes an element from a queue implemented using an array.

## Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



## Program:
```
int front, rear;
void dequeue()
{
    front ++;
}
```

## Output:

![image](https://github.com/user-attachments/assets/ef75dd76-4168-412a-9599-29af6fbf0eb1)

## Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
