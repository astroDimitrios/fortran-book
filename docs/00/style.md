# Code Style

```{contents}
:local:
```

Having a consistent code style improves readability and makes collaboration easier. This book follows the code style outlined below; if your organisation has its own code style then use it! Some of the style relates to topics you haven't seen in this book yet. Best practice and code styling will be pointed out in future lessons.

INC SHORT EXAMPLE?  
DO WE WANT A STYLE ADMONITION?  
INCLUDE STYLIST INFO <https://github.com/MetOffice/stylist>

## Basics

- Short and simple Fortran statements are easier to read and understand than long and complex ones
- Files should have a header with copyright, all blank lines in the copyright should start with `!`
- Write your program in UK English
- use lower case only, except for physical constants: `Rd`
- Optional spaces should be used for readability: `end if` not `endif`
- End statements should be named: `end subroutine test`

## Variables

- Declare and comment variables
- Use `snake_case` for names NOT camelCase
- Function arguments should be declared separately to local variables
- Avoid the use of ‘magic numbers’ that is numeric constants hard wired into the code. Use parameters instead.
- Literal real values must always be given a kind using this syntax: `myvar = 1.23_r_mykind`

## General

- `exit` statements must be labelled
- Label nested loops to improve readability
- The continued line marker `&` should be aligned
