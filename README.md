# logic-sourcecode-lab-bug-error-warning
logic-sourcecode-lab-bug-error-warning created by GitHub Classroom
---------
## Step I: Select method
```
/**
 * Checks if a given file is PDF
 * @param file - input file
 * @return tru - if condition satistfies, else false
 */
private boolean isPDFAndNotDirectory(File file) {
    return !file.isDirectory() &&
            file.getName().endsWith(mContext.getString(R.string.pdf_ext));
}
```

## Step 2:
1. Simplify: a && b  
2. Get Predicate Coverage: p = a && b  
  Make p = true, a = true, b= true  
  Make p = false, a = false, b= false  

## Step 3: Get Clause Coverage
p = a && b, Make each clause true & false  
a = true, b= true  
a = false, b= false  

## Step 4: Get Combinatorial Coverage

| a | b | p |
|:-:|:-:|:-:|
| T | T | T |
| T | F | F |
| F | T | F |
| F | F | F |

