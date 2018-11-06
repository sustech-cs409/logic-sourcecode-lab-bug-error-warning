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
