package com.company;  
  
import java.util.Scanner;  
  
public class Main {  
  
    public static void main(String[] args) {  
        Scanner sc =new Scanner(System.in);  
        while ((sc.hasNext())){  
           String str=sc.nextLine();  
           if(str.equals("0"))  
               break;  
             char[]arr=str.toCharArray();  
             int odd=0,even=0,n;  
             for(int i=0;i<arr.length;i++){  
                 if(i%2==0) {  
                     odd +=arr[i]-'0';  
                 }else{  
                     even +=arr[i]-'0';  
                     }  
                 if((even-odd)%11==0){  
                     System.out.println(str+"is a multiple of 11");  
                 }else{  
                     System.out.println(str+"is not a multiple of 11");  
                 }  
             }  
        }  
    }  
}  
