#include<stdio.h>
#include<stdlib.h>

struct Node
{
  int data;
  struct Node *next;
};
void
LinkedListTransversal (struct Node *ptr)
{
  while (ptr!=NULL)
    {
      printf("Elements :%d\n", ptr->data);
      ptr = ptr->next;
    }
}
//case1:delete first Node
struct Node *deletefirstnode(struct Node *head){
 struct Node *ptr=head;
 head=head->next;
 free(ptr);
 return head;
}

int
main ()
{
  struct Node *head;
  struct Node *second;
  struct Node *third;
  struct Node *fourth;

  //Allocating memory in the link list in heap
  head = (struct Node *) malloc (sizeof (struct Node));
  second = (struct Node *) malloc (sizeof (struct Node));
  third = (struct Node *) malloc (sizeof (struct Node));
  fourth = (struct Node *) malloc (sizeof (struct Node));

  //linking head ans second
  head->data = 17;
  head->next = second;

  //linking second to third
  second->data = 15;
  second->next = third;

  //linking third to fourth
  third->data = 20;
  third->next = fourth;

  //terminating list at fourth 
  fourth->data = 45;
  fourth->next = NULL;

  printf("\nlist before deletion\n");
  LinkedListTransversal (head);
   
   head=deletefirstnode(head);
   printf("\nlist after deletion\n");
  LinkedListTransversal (head);
   
   
  return 0;

}
