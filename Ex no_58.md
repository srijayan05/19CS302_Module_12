# EX 58 C Function to display queue elements using Linked List.(use float data in the queue)
## DATE:
## AIM:
To write a C Function to display queue elements using Linked List.

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
void display()
{
    struct Node *ptr;
    ptr=front;
    if(front==NULL)
    {
        printf("queue is empty");
        
    }
    else
 {
    printf("Queue elements:\n");
    while(ptr!=0)
    {
        printf("%.3f\n",ptr->data);
        ptr=ptr->next;
    }
  }
}
```

## Output:
![Screenshot 2025-05-08 101018](https://github.com/user-attachments/assets/dbe7949a-16a1-41e9-886f-b9361833b6db)




## Result:
Thus the program was executed and the output was verified successfully.
