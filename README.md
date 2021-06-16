# unbxd
UNBXD ASSESSMENT ANSWERS

1.	D   (a, 2) (b, 4) (c, 1) (d, 3)
2.	B    Prints all nodes in reverse order
3.	A   an array of 50 numbers
4.	B   Transpose of matrix A
5.	A    Context switch
6.	D   all
7.	D  o(n^2log(n))
8.	1 Billion characters
9.	A program counter
10.	A stack
11.	B     Recurrence is T(n) = T(n-1) + O(n) and time complexity is O(n^2)
12.	C    O(n)
13.	A O(logn)
14.	A Merge sort
15.	A SMTP
16.	B n=21, k=12
17.	B STACK
18.	C  QMNPRO

2) import java.util.Arrays;
import java.util.Scanner;


public class shuffle {
   static int countadding(int n)
   {
       int list[] = new int[n + 1];
       Arrays.fill(list, 0);
       list[0] = 1;
       for (int i = 1; i < n; i++)
           for (int j = i; j <= n; j++)
               list[j] += list[j - i];
   
       return list[n];
   }
   public static void main (String[] args)
   {
       Scanner s = new Scanner(System.in);
    System.out.print("Enter the number: ");
       int n = s.nextInt();
       System.out.print(countadding(n));
   }
}


1) #include<stdio.h>

int arrange(*linked_list head)
{
    int len=0
    struct linked_list *p=head,*mid=head;
    for(p){
        len=len+2;
        p=p->next;
        p=p->next;
        mid=mid->next;
    }
    int arr[100];
    p=head
    for i=0;i<len;i++{
        if(i%2 != 0){
            arr[i]=mid->data
            mid=mid->next
        }
        else{
            arr[i]=p->data
            p=p->next
        }
    }
    p=head;
    for i=0;i<len;i++{
        p->data=arr[i]
    }
}
