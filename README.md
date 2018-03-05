# This is an <h1> tag #
## This is an <h2> tag ##
###### This is an <h6> tag ######

**Bold** and *italic* text
* Item 1
* Item 2
  * Item 2a
  * Item 2b
  
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
   
   ![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)

http://github.com - automatic!
[GitHub](http://github.com)

As Kanye West said:

> We're living the future so
> the present is our past.

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
```prolog
PREDICATES
  factorial(unsigned, long)
CLAUSES
  factorial(1,1). % Факториал от 1 равен 1. 5.
  factorial(N,FN):─ % Чтобы вычислить факториал числа N, надо вычислить   
  NewN=N-1, % факториал числа N-1 и умножить его на N. 
  factorial(NewN,Ft), 
  FN = N*Ft. 
GOAL  
  X=3, factorial(X,FX).  
``` 
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

#1
mojombo#1
mojombo/github-flavored-markdown#1

:pig2::dash::dash:
