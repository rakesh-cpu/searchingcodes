# searchingcode in python
def linears(list,key):
    n=len(list);
    for i in range(n):
        if list[i]==key:
            flag=1
        else:
            flag=0
        if(flag==1):
            print("element found at index",i)
list=[2,4,4,32,1,4,5,6,7]
key = int(input("enter a search key:"))
linears(list,key)

#linearsearch in java
import java.util.*;
public class Linearsearch{
    
    public static void linears(int arr[],int key){
        int flag=0;
        int n = arr.length;
        for(int i=0;i<n;i++){
            if(arr[i]==key){
                //System.out.println("your searching element found at index:"+i);
                flag=1;
            }
            else{
                 flag=-1;
            }
            if(flag==1){
                System.out.println("your searching element found at index:"+i);
            }
            
        }
        
        
    }
    public static void main(String args[]){
        Linearsearch ls = new Linearsearch();
        
        int arr[]={2,53,2,4,53,6,73,2,12,34,5};
        System.out.println("enter search key:");
        Scanner sc = new Scanner(System.in);
        int key = sc.nextInt();
        linears(arr,key);
        
    }
}
