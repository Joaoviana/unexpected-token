# unexpected-token. (syntax error)

When JavaScript engine cannot parse the file beacuse I made an error in my code. It cannot even make it past the creation phase. 

More specifically, I started something I didn't finish. Opened parenthesis I never closed, used and operator with no operand

I first came across this error studying type coercion when I tried to void the typeof operator. I expect this error will be a real pain because the message is not very helpful. 

It tells me there is something missing, but always 

I'll have to go back through the WHOLE FILE to find where I made my mistake.

___

#code where I first found the error

```js

typeof void

//comments
```

```js

typeof void;

//comments
```

These look so similar, but are so different. with the semicolon JS catches the error before moving on to the rest of the file. 
this way it can tell me the error is on line, instead of having to stumble to the end and tell me something unhelpful. 

___

# The Fixe

well, void is an operator. it requeires a value to its left, so i gave it one. 

```js
type of void null;
```

_null_ for fun, but it could be anything. it does not matter. _void_ turns anything to _undefined_.

___

## Messages from different runtimes

...todo

___

## More instances

ongoing. (almost) everytime you come cross itm copy-paste the code onto this repo. 
