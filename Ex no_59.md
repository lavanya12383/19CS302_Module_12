# EX 59 C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.(use character data in Queue).
## DATE:17/3/26
## AIM:
To write a C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.

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
## Program:
```
/*
functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.(use character data in Queue).
struct Node
{
   float data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void enqueue(float data)
{
    struct Node *ptr=(struct Node*)malloc(sizeof(struct Node*));
    ptr->data=data;
    ptr->next=NULL;
    if(front == NULL)
    {
        front=rear=ptr;
    }
    else
    {
        rear->next=ptr;
        rear=ptr;
    }
}
void display()
{
    printf("queue elements:\n");
    struct Node *ptr;
    ptr=front;
    while(ptr!=NULL)
    {
        printf("%.3f\n",ptr->data);
        ptr=ptr->next;
    }
}
void dequeue()
{
    struct Node *ptr;
    if(front==NULL)
    {
       printf("queue is empty"); 
    }
    else
    {
        ptr=front;
        front=ptr->next;
        free(ptr);
    }
    
}
void peek()
{
    printf("peek:%.3f\n",front->data);
} 
*/
```

## Output:
<img width="676" height="1005" alt="image" src="https://github.com/user-attachments/assets/3da2bb43-f176-4a8d-a038-3b95a32ffdff" />



## Result:
Thus the program was executed and the output was verified successfully.
