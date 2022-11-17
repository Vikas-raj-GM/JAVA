import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    static int m, n;
          static  int arr[] = new int[200];
        static int pos[] = new int[200];
    
    public static void main(String[] args) {
        int t, i;

        
        Scanner sc = new Scanner(System.in);
        t = sc.nextInt();
        while(t-- >0)
        {
            n = sc.nextInt();
            m = sc.nextInt();
            
            for(i=0; i<n; i++)
                arr[i] = sc.nextInt();
            
            for(i=0; i<n; i++)
                pos[i] = 0;
            
            if(foo(0))
                System.out.println("YES");
            else
                System.out.println("NO");
                
        }
    }
    
    public static boolean foo(int index)
    {        
        boolean result = false;
        
        if(index+1 >= n || index + m >= n)
            return true;
        
        if(arr[index+1] == 0 && pos[index+1]==0)
            {
            pos[index+1]=1;
            result |= foo(index+1);                        
        }
        if(arr[index+m] == 0 && pos[index+m]==0) 
            {
            pos[index+m]=1;
            result |= foo(index+m);                
        }
        if(index>0 && arr[index-1]==0 && pos[index-1]==0)        
            {
            pos[index-1]=1;
            result |= foo(index-1);
        }   
        return result;
        
    }
    
}
