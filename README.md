# linked_list


void append()
{

    struct node* temp;
    temp=(struct node*) malloc(sizeof(struct node));
    printf("enter node data");
    scanf("%d",&temp->data);
    temp->link=NULL;
    if(root==NULL) //list is empty
    {

        root=temp;
    }
    else
    {

        struct node* p;
        p=root;
        while(p->link!=NULL)
        {


          p= p->link;
        }
        p->link=temp;
    }
}
