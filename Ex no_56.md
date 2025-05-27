# EX 56 A function to display stack elements using Linked List.(store float data in stack).
## DATE:
## AIM:
To write a C function to display stack elements using Linked List.

## Algorithm:
1. Start. 
2. Define a variables. 
3. Write a program to display stack elements using linked list. 
4. Read the value using scanf. 
5. Ask the user to make an input. 
6. Print out the answer. 
7. End 
## Program:
```
Struct Node 
{ 
  int data; 
  struct Node *next; 
}*head; 
void display() 
{ 
  struct Node *temp= head; 
  while(temp!=NULL) 
  { 
    printf("%d\n",temp->data); 
    temp=temp->next; 
  } 
}
```
## Output:
![Screenshot 2025-05-08 100433](https://github.com/user-attachments/assets/fc6c31af-1d68-4f61-8ed4-9b0dbe8b9822)


## Result:
Thus the program was executed and the output was verified successfully.
