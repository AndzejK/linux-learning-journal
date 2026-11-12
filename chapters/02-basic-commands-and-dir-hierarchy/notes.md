## Navigating Directories

**Root Directory**: The Unix directory hierarchy starts at '**/**'.

## Variables (Shell VS Environment)
- **Shell var**: a *value* that belongs to my **current** shell
- **Env var**: a *value* that can be passed down to a program by my open shell session:
```bash
EXPORT 
``` # exposes the var to global (env) scope
```bash
#!/bin/bash
export DEPLOY_ENV="PROD"
echo "Deploying to: $DEPLOY_ENV"
``` 

**Note**: Do Not put any space around the *=* when assingning a var!
