# Reverse_a_String
Reverse a String using stack...(Java Collection Framework)
//# Code Solution...
import java.util.*;
class StackB {
  
        static String reverse(String str)
        {
            Stack<Character> s = new Stack();
            int idx=0;
            while(idx<str.length())
            {
                s.push(str.charAt(idx));
                idx++;
            }
            StringBuilder sb = new StringBuilder("");
            while(!s.isEmpty())
            {
                char curr = s.pop();
                sb.append(curr);
                
            }
            return sb.toString();
            
        }
    
    
    public static void main(String[] args) 
    {
       String str="Shantanu";
       String p=reverse(str);
       System.out.print(p);
    }
}
