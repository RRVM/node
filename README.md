#include <stdio.h>
#include<bits/stdc++.h>
using namespace std;
struct node* bstnode(struct node* root)
{
    struct node* ownername=NULL;
    struct node* address=NULL;
    struct node* mobile=NULL;
    struct node* phone=NULL;
    struct node* value=NULL;
    struct node* childnumber=NULL;
    char name;
    char addr;
    int mob;
    int phon;
    float val;
    int nodenumber;
}
struct node* newnode(bstnode* root,char name,char addr,int mob,int phon,float val,int nodenumber)
{
    struct bstnode* newnode=new newnode;
    newnode->ownername=name;    /* for entering owner name*/
    
    newnode->address=addr;      // for entering address
    
    newnode->mobile=mob;        //for entering mobile number
   
    newnode->phone=phon;        // for entering phone number
    
    newnode->value=val;         // for entering value

    newnode->childnumber=nodenumber;     // for nodenumber
    
}
int main()
{
    struct bstnode* root;                                         //task: 1
    
    
    cout<<"enter owner name, address, mobile, phone, value";
    cin>>name>>addr>>mob>>phon>>val;                  
    root->nodenumber=newnode(root,name,addr,mob,phon,val,1);      //task: 2
    
    
    cout<<"enter owner name, address, mobile, phone, value";
    cin>>name>>addr>>mob>>phon>>val;


    cout<<"enter nodenumber";                                     // task:3
    cin>>nodenumber;
    cout<<"enter owner name, address, mobile, phone, value";
    cin>>name>>addr>>mob>>phon>>val;   
    root->nodenumber=newnode(root,name,addr,mob,val,nodenumber);
    
    
    int password,n;                                              //task: 4
    cout<<"enter nodenumber of the node you want to print values of";
    cin>>n;
    int encryptedpass=n*111;
    cout<<"enter password of the node youwant to print values of";
    cin>>password;
    if(password==encryptedpass)
    print(root,nodenumber);
    
    
    cout<<"enter the nodenumber you are owner of";              // task: 5
    cin>>n;
    int encryowner=213*n+10;
    cout<<"enter password of the node you are the qwner of";
    int pass;
    cin>>pass;
    if(pass==encryowner)
    cout<<"owner verified";
    else
    cout<<"wrong access";
    
    
    cout<<"enter the nodenumber you are owner of";              // task: 6
    cin>>n;
    int encryowner=213*n+10;
    cout<<"enter password of the node you are the qwner of";
    int pass;
    cin>>pass;
    if(pass==encryowner)
    cout<<"you can break down the node";
    else
    cout<<"wrong access";
    
    cout<<"enter the nodenumber you are owner of";              // task: 7
    cin>>n;
    int encryowner=213*n+10;
    cout<<"enter password of the node you are the qwner of";
    int pass;
    cin>>pass;
    if(pass==encryowner)
    {
        cout<<"enter the name of new owner";
        char owr;
        cin>>owr;
        cout<<"enter new owner";
        root->nodenumber=newnode(root,name,addr,mob,phon,val,1);
    }
    else
    cout<<"wrong access";
}  

