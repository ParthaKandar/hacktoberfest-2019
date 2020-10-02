# show you some code using java
# this is my first repository 

# factorial using java :

class Fact{  
 public static void main(String args[]){  
  int i,fact=1;  
  int number=5;    
  for(i=1;i<=number;i++){    
      fact=fact*i;    
  }    
  System.out.println("Factorial of "+number+" is: "+fact);    
 }  
}  

# find perfect no using java :

import java.util.Scanner;

public class PerfectNumberUsingFor {
	private static Scanner sc;
	
	public static void main(String[] args) {
		int i, Number, Sum = 0 ;
		sc = new Scanner(System.in);		
		System.out.println("\n Please Enter any Number: ");
		Number = sc.nextInt();

		for(i = 1 ; i < Number ; i++) {
			if(Number % i == 0)  {
				Sum = Sum + i;
			}
		}
		if (Sum == Number) {
			System.out.format("\n% d is a Perfect Number", Number);
		}
		else {
			System.out.format("\n% d is NOT a Perfect Number", Number);
		}
	}
}

# Frequency of a word :

public class Main 
{ 
    public static void main(String[] args) 
    {        
        String text = "the quick brown fox jumps fox fox over the lazy dog brown"; 
        String[] keys = text.split(" "); 
        String[] uniqueKeys; 
        int count = 0; 
        System.out.println(text); 
        uniqueKeys = getUniqueKeys(keys); 
        for(String key: uniqueKeys) 
        { 
            if(null == key) 
            { 
                break; 
            }            
            for(String s : keys) 
            { 
                if(key.equals(s)) 
                { 
                    count++; 
                }                
            } 
            System.out.println("Count of ["+key+"] is : "+count); 
            count=0; 
        } 
    } 
    private static String[] getUniqueKeys(String[] keys) 
    { 
        String[] uniqueKeys = new String[keys.length]; 
        uniqueKeys[0] = keys[0]; 
        int uniqueKeyIndex = 1; 
        boolean keyAlreadyExists = false; 
        for(int i=1; i<keys.length ; i++) 
        { 
            for(int j=0; j<=uniqueKeyIndex; j++) 
            { 
                if(keys[i].equals(uniqueKeys[j])) 
                { 
                    keyAlreadyExists = true; 
                } 
            }            
            if(!keyAlreadyExists) 
            { 
                uniqueKeys[uniqueKeyIndex] = keys[i]; 
                uniqueKeyIndex++;                
            } 
            keyAlreadyExists = false; 
        }        
        return uniqueKeys; 
    } 
} 

# thank you i hope it helps you in the future.