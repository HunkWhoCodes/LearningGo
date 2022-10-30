## Go Syntax:

### Syntax Rules
- GO is case sensitive.
- Names of public fields have initial uppercase letters.
- Initial uppercase in GO means that the symbol is exported and is same as saying that it is public.

#### Semicolon and Ending Statments in GO
- A statement is terminated by a new line and no semicolon is required.
- Though the language specification asks for semiclons.
- The Lexer software component that analyzes and parses the code, adds them during compilation.
- So GO is sensitive to whitespace like tabs, spaces, new lines etc.
- So if there is a multi line statement, it can be misinterpreted by lexer as multiple statements.

#### Code Blocks With Braces
- Code Blocks are wrapped with braces like C and Java

```go
  sum := 0
  for i := 0; i < 10; i++ {
    sum += i
  }
  
  fmt.Println(sum)  // Prints 45
```

- The starting brace i.e. `{` must be on the same line where the code block begins
- This is because otherwise, the white space will be considered as termianted loop i.e. : `for i := 0; i < 10; i++`
- This is unlike Java or C++ where whitespace has no significance, so it doesn't matter if the openig brace is in the same line or in next line.

### Built in Functions:
- These functions are always available and don't need to be imported.
- These are part of a package called `builtin`.
- Complete list is available at: [Package builtin](https://pkg.go.dev/builtin)
- Some examples are:
  - len(string) : returns the length fo the string.
  - panic(error) : stops execution and displays an error message 
  - recover : To manage the behaviro of a panicking routine

