<!--comment-->
r _e_~~c~~t `angle`
---

<p>// write a programme that print rectangle</p>

```c
#include<stdio.h>
int main()
{
    int num,col,row;
    printf("Enter the number = ");
    scanf("%d",&num);

    for(row=1; row<=num; row++)
    {
        for(col=1; col<=num; col++)
        {
            if(row==1 || row==num || col==1 || col==num)
            printf("%d",col);
        else
        printf("*");
        }
        printf("\n");
    }
}
```

<image src="./images/prac.png" width="400" title="onedigit"/>

### with space

`printf(" ");`

![demot](./images/space.png)

<p> // rectangle after 9 too </p> 

### Perfect rectangle

```c
#include<stdio.h>
int main()
{
    while(1)
    {
        int num,col,row;
        printf("Enter the number = ");
        scanf("%d",&num);

        for(row=1; row<=num; row++)
        {
            for(col=1; col<=num; col++)
            {
                if(row==1 || row==num || col==1 || col==num)
                printf("%d",col);
                else
                    if(col<=9)
                    printf("#");

                else
                    printf("**");
            }
            printf("\n");
        }
    }
}
```
![demo](./images/rectangle.png)

### with space
`if(col<=9)`</br>
`printf(" ");`</br>
`else`  
`printf("  ");`  

![pic](./images/withspace.png)

<image src="./images/perfectspace.png" width="500" title="perfect space"/>

### rectangle with star

`printf("*",col);`

<image src="./images/star.png" width="500" title="star"/>

### rectangle with unlimited row column using Hesh

```c
#include<stdio.h>
int main()
{
    while(1)
    {
        int rnum,cnum,col,row;
        printf("Enter the row number = ");
        scanf("%d",&rnum);
        printf("Enter the column number : ");
        scanf("%d",&cnum);

        for(row=1; row<=rnum; row++)
        {
            for(col=1; col<=cnum; col++)
            {
                if(row==1 || row==rnum || col==1 || col==cnum)
                    printf("#",col);
                else
                    printf(" ");
            }
            printf("\n");
        }
    }
}
```
![heash](./images/heash.png)

### alphabet

```c
#include<stdio.h>
int main()
{
    while(1)
    {
        int rnum,cnum,col,row;
        printf("Enter the row number = ");
        scanf("%d",&rnum);
        printf("Enter the column number : ");
        scanf("%d",&cnum);

        for(row=1; row<=rnum; row++)
        {
            for(col=1; col<=cnum; col++)
            {
                if(row==1 || row==rnum)
                    printf("%c",row+64);
                    else if(col==1 || col==cnum)
                        printf("%c",col+64);
                else
                    printf(" ");
            }
            printf("\n");
        }
    }
}

```

<image src="./images/alphabet.png" width="500" title="alphabet"/>

### exchange the col & row

`if(row==1 || row==rnum)`  
    `printf("%c",col+64);`  
`else if(col==1 || col==cnum)`  
`printf("%c",row+64);`  

![allalphabet](./images/allalphabet.png)

_continue_