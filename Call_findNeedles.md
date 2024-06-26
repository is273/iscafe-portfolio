# Call Method: findNeedles
Calls the [findNeedles method](https://docs.google.com/document/d/1zeIYLWabTiahjGU6y6IfVxcwv8XNJg_sTfMbBNyxs70/edit) 
and compares the values of the `haystack` string
and the `needles` string array.

Returns the number of times a value appears in the `haystack` string.

## Request Body
The request body contains data with the following structure:

```
public class FarmBarn{ 
    public static void main(String[] args){ 
        String[] needles={"almost", "knew", "ground", "sky"};
        String haystack=("almost before we knew it, we had left the ground");
        findNeedles(haystack, needles);
    }
```

## Fields
| Field  | Description |
| ------------- | ------------- |
| `public class`  | The name of the public class.|
| `public static void`  | Stores the Java command line arguments in an array.|
| `String[] needles` | The values stored in a string array to be compared.|
| `String haystack` | The value stored in a string to be compared.|

## Response Body
If successful, each term from the `needles` string array shows with the number 
of times each term appears in the `haystack` string.

If the `needles` string array’s length is greater than 5, the function prints an error and exit.
