### Syntax Rules
- GO is a case sensitive.
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


