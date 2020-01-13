# Chip

A template-based file generator, since cookie cutter does not support this yet!

## Usage
`chip [PATH/TO/TEMPLATE]`

## Templates

Templating works similarly to cookie cutter, in the sense that you designate a template term inside of `{{ term }}`

e.g.
```
class {{ CLASSNAME }} {  
    constructor() { . 
      this.name = {{ NAME }}  
      this.age = {{ AGE }} . 
    }
 }
```

Then, you will be asked for the value for CLASSNAME, NAME, AGE

### Modifiers

In templates you can specify a modifier:
* lower - `{{ PLACEHOLDER.lower }}` - value entered for `PLACEHOLDER` **lowercased**
* upper - `{{ PLACEHOLDER.upper }}` - value entered for `PLACEHOLDER` **uppercased**
* capitalize - `{{ PLACEHOLDER.capitalize }}` - value entered for `PLACEHOLDER` **capitalized**

## Installation

`sudo make install` will install this into `/usr/local/bin` which should already be in your PATH.
