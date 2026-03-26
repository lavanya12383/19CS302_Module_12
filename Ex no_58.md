# EX 58 C Function to display queue elements using Linked List.(use integer data in the queue)
## DATE:
## AIM:
To write a C Function to display queue elements using Linked List.

## Algorithm
Start
Define a structure Node with two fields:
data (integer type)
next (pointer to the next node)
Initialize front and rear pointers:
front points to the first node in the queue
rear points to the last node in the queue
Check if front is NULL:
If NULL, print "Queue is empty" and exit.
Otherwise, create a temporary pointer temp pointing to front.
Loop through the queue:
Print temp->data.
Move temp to temp->next.
Continue until temp becomes NULL.
End
This algorithm efficiently traverses and prints all queue elements using a linked list. Want a full implementation with enqueue and dequeue functions? 🚀
## Program:
```
/*
C Function to display queue elements using Linked List.(use integer data in the queue)

struct Node
{
   float data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void display()
{
    struct Node *ptr;
    ptr=front;
    if(front==NULL)
    {
        printf("queue is empty");
        
    }
    else
    {printf("Queue elements:\n");
    while(ptr!=0)
    {
        printf("%.3f\n",ptr->data);
        ptr=ptr->next;
    }}
}
*/
```

## Output:

<img width="888" height="541" alt="image" src="https://github.com/user-attachments/assets/bb97e19e-b0bf-4296-b478-b0aa21622402" />


## Result:
Thus the program was executed and the output was verified successfully.
