# EX 59 C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.(use float data in Queue).
## DATE:
## AIM:
To write a C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.

## Algorithm:
1. Start
2. Define a structure `Node` with two fields:  
   - `data` (integer type)  
   - `next` (pointer to the next node)  
3. Initialize `front` and `rear` pointers:  
   - `front` points to the first node in the queue  
   - `rear` points to the last node in the queue  
4. Check if `front` is `NULL`:  
   - If `NULL`, print "Queue is empty" and exit.  
5. Otherwise, create a temporary pointer `temp` pointing to `front`.  
6. Loop through the queue:  
   - Print `temp->data`.  
   - Move `temp` to `temp->next`.  
7. Continue until `temp` becomes `NULL`.  
8. End 


## Program:
```
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
```

## Output:
![Screenshot 2025-05-08 101233](https://github.com/user-attachments/assets/139f0b93-cb89-4cc8-a8f2-359a9dacd53d)


## Result:
Thus the program was executed and the output was verified successfully.
