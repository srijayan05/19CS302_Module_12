# EX 60 C function to find the peek element of the queue using linked list.
## DATE:
## AIM:
To write a C function to find the peek element of the queue using linked list.

## Algorithm:
1. Start  
2. Check if the queue is empty (`front == NULL`):  
   - If empty, print "Queue is empty" and exit.  
3. Otherwise, return the `data` of the `front` node.  
4. End 

## Program:
```
struct Node
{
   int data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void peek()
{
    printf("%c",front->data);
}
```

## Output:
![Screenshot 2025-05-08 101447](https://github.com/user-attachments/assets/f15ed0e4-d5e3-4910-a405-ab0fcefcf001)



## Result:
Thus the program was executed and the output was verified successfully.
