# C10
Memory allocation #include<stdio.h>
struct student {
char name[50];
int age ;
float marks;
};
int main(){
struct student *ptr;
ptr=(struct student*)malloc(sizeof(struct student));
if(ptr==NULL){
printf ("memory allocation failed \n");
return 1;
}
printf ("enter name:");
scanf("%s",&ptr->name);
printf ("enter age:");
scanf ("%d",&ptr->age);
printf ("enter marks:");
scanf("%f",&ptr->marks);
printf ("student details: \n");
printf ("name:%s\n age:%d\n marks:%.2f\n",ptr->name,ptr->age,ptr->marks);
free(ptr);
return 0 ;
}

