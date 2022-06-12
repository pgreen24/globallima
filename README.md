File create in c

int main(){
FILE*file;#include<stdio.h>

char name[20] ="Rabeya Akter";
int length = strlen(name);
int i;
file=fopen("lima.leo","a");
if(file==NULL)
{
    printf("file is exit");
}
else{
    printf("file is open\n");
    for(i=0;i<length;i++);
    {
        fputc(name[i],file);
    }
    printf("file is reten successsfully\n");
    fclose(file);
}
getch();
}

