# SoulsLang

Kind of language I am working towards.
Closer to writing algebra but the computer understands.

A language which is written in sanskrit and follows the way sanskrit sees the world. Not a sanskrit syntax wrapper around C.

Example:

1.
```normal
result = add(a, b);
```
```SoulsLang
कर्ता: a  कर्म: b  क्रिया: जोड़  फल: result |
```

2
```java
account.transfer(amount, recipient);
```
```SoulsLang
कर्ता: sender  कर्म: amount  सम्प्रदान: recipient  क्रिया: transfer |
```
in any order cause it's never order we are focusing as each object itself describes what it's purpose is.

here you can have full syntax power of a normal lang. You don't just write add, you define add function and when it sees the semantic  attached to it, then it is searched and so and so.

Basically semantic dispatch.
something like this

```SoulsLang
क्रिया जोड़:
    कर्ता: संख्या  कर्म: संख्या  →  संख्या |
    
क्रिया जोड़:
    कर्ता: सूची  कर्म: संख्या  →  सूची |
```
So it's not just another SQL or any such declarative type, user can define their own relations. More of type theory.

The relationship owns the operation, not any single participant

var declaration would be like this

```soulslang
नाम: a  प्रकार: संख्या |
```

also we would likely have a simplistic layer like := and + instead of jor but yea.

Current idea is to use Ocaml as it have good type system.


It's just rough draft for now a 4am rambling would refine as we go along.
