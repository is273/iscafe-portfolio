# Method: findNeedles
The findNeedles method can compare the values of the `haystack` string and the `needles` string array. The findNeedles method returns the number of times a value appears in the `haystack` string.

## Request Body
The following is an example of the structure of the request body: 

```
public class FarmBarn{ 
    public static void main(String[] args){ 
        String[] needles={"almost", "knew", "ground", "sky"};
        String haystack=("almost before we knew it, we had left the ground");
        findNeedles(haystack, needles);
    }
    public static void findNeedles(String haystack, String[]  needles){  
        if (needles.length>5){ 
            System.err.println("Too many words!");
        }else{ 
            int[] countArray=new int[needles.length];
            for (int i=0; i<needles.length; i++) {
                String[] words=haystack.split("[ \"\'\t\n\b\f\r]", 0);
                for (int j=0; j<words.length; j++) {
                    if (words[j].compareTo(needles[i])==0) {
                        countArray[i]++; 
                    }
                }
            }
            for (int j=0; j < needles.length; j++){  
                System.out.println(needles[j]+": "+countArray[j]);
            }
        }
    }
}
```

## Fields
| Field  | Description |
| ------------- | ------------- |
| `public class`  | The name of the public class.|
| `public static void`  | Stores Java command-line arguments in an array.|
| `String[] needles`  | The values that are stored in a string array to be compared.|
| `String haystack`  | The value that is stored in a string to be compared.|
| `public static void`  | The name of the method and its parameters.|
| `int[] countArray`  | Stores the length of the needle string array.|
| `String[] words`  | Breaks the haystack string based on the delimiters and limit.|
| `System.err.println`  | The error that prints if the method fails.|
| `System.out.println`  | The message the method prints.|

## Response Body
After calling the method, each term from the needles string array will 
show with the number of times the term appears in the haystack string.
If the needles string array’s length is greater than 5, the method prints an error and exits.
