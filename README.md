# singly-linked-list-traversing
#include <iostream>

using namespace std;

class node{
    public:
    int data;
    node *next;
};
void display(node *temp)
{
    while(temp!=NULL)
    {
        cout<<temp->data<<" ";
        temp=temp->next;
    }
}
    int main()
{
    node *head=NULL;
    node *second=NULL;
    node *third=NULL;
    //ALOCATE MEMRY
    head=new node();
    second=new node();
    third=new node();
    //data
    head->data=1;
    head->next=second;
    second->data=2;
    second->next=third;
    third->data=3;
    third->next=NULL;
    display(head);
      }
