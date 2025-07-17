#this is backend project
## Git Error: src refspec main does not match any

If you see this error when pushing to GitHub:

```
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/bvishal-27/Backend-.git'
```

**Possible cause:**  
You have created a new branch (`main`), but you haven't made any commits yet. Git cannot push an empty branch.

**How to fix:**
1. Add a file or make a change:
    ```bash
    echo "# Backend Project" > README.md
    git add README.md
    git commit -m "Initial commit"
    ```
2. Push the branch:
    ```bash
    git push origin main
    ```

This should resolve the error.  