### Commit Message Header

```
<type>(scope): <short-summary>
  │       │             │
  │       │             └─⫸ Summary in present tense. Not capitalized. No period at the end.
  │       │
  │       └─⫸ Commit Scope: users-mgmt|tours-mgmt|payments|study-programs|transactions              
  │                          
  │
  └─⫸ Commit Type: build|ci|docs|feat|fix|perf|refactor|test
```

```
feat(users-mgmt): add new button
```

#### `<type>`
* `build`: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
* `ci`: Changes to our CI configuration files and scripts (examples: CircleCi, SauceLabs)
* `docs`: Documentation only changes
* `feat`: A new feature
* `fix`: A bug fix
* `perf`: A code change that improves performance
* `refactor`: A code change that neither fixes a bug nor adds a feature
* `test`: Adding missing tests or correcting existing tests


#### `(scope)`
* `users-mgmt` 
  * user; role; permission
* `tours-mgmt`
  * tour; tour-guide; booking; tour-schedule
* `payments`
  * payment; invoice
* `study-programs`
  * program; course; materials
* `transactions`
  * users-logs; 

#### `<short-summary>` 

> Use the summary field to provide a succinct description of the change:

* `add` - introduce new func or files
* `fix` - correct a bugs or issue
* `update` - bring something up to date, such as dependencies or docs
* `remove` - eliminate unnecessary coee or files
* `improve` - enhance performance, readability or efficiency
* `implement` - complete the implementation of a feature or functionality
* `optimize` - improve the performance or efficiency of code
* `change` - modify behavior or structure
* `configure` - set up or adjust settings and configurations
* `test` - add or improve test cases
* `revert` - undo a previous commit or change
* `resolve` - solve a merge conflict or issue
* `merge` - combine changes from different branches 
