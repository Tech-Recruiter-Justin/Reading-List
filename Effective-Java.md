# Effective Java - Key Takeaway

## Foreword
The three things to master in a language:
1. How the language is structured (grammar)
2. How to name things you wnat to talk about (vocab)
3. The customary and effective ways to say everyday things (usage) <- this book

Java is:
- Object-oriented with single inheritance
- Supports an imperative (statement-oriented) coding style
- The libraries address graphic display support, networking, distributed computing, and security

## Creating and Destroying Objects
### Static factory methods instead of constructors
|   | Static Factory Methods  | Constructors|
| :------------: | :------------: | :------------: |
| Naming | yes, easier to understand  | none, unless the parameters are descriptive |
| Variance | yes, can create multiple methods with different names  | there should only be one constructor for each class |
| Must create new object? | no, allows instance-controlled classes, saves resources | yes, may create unnecessary duplicate objects and expensive  |
| Singleton | Yes | No |
| Noninstantiable | Yes | No |
| No two equal instances exist | Yes | No |
| Can return an object of any subtype | Yes, can hide implementation classes | No |
| No two equal instances exist | Yes | No |
| No two equal instances exist | Yes | No |
can return an object of any subtype


ADVANTAGE:
- they have names so they are easier to understand VS parameters without names
- there can be multiple static factory methods in one class VS there can only be one constructor (bypassing using different parameter is hard to remember)
