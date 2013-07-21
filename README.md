Plus-One
========


public class Solution {
    public int[] plusOne(int[] digits) {
        // Start typing your Java solution below
        // DO NOT write main() function
        
        if(digits == null) return null;
        
        int end = digits.length-1;
        
        
        
        while(end >=0){
            
        int sum = digits[end] + 1;
            
        if(sum == 10){
            digits[end] = 0;
            
            end --;
        }
        
        else{
            digits[end] = sum;
            break;
        }
        }
        
        if(end <0){
            
            int[] result = new int[digits.length+1];
            result[0] = 1;
            
            for(int i = 1; i < result.length;i++){
                result[i] = 0;
            }
            
            return result;
        }
        
      
        return digits;
       
    }
}
