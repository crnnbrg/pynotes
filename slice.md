---
layout: post
title: "Welcome to Jekyll!"
toc: true
---
> variable[start:end + 1]

# Slice
works with list, string or tuple

```python
s = "Hello"
```

```
 H  e  l  l  o
 0  1  2  3  4
-5 -4 -3 -2 -1
```
|Slice|result|explanation|
| ----|:---:|---|
s[1:4] |'ell'|chars starting at index 1 and extending up to but not including index4.|
s[1:] |'ello'| omitting either index defaults to the start or end of the string.|
s[:1] |'H'| start from the beggining and stop at index 1|
s[:] |'Hello'| omitting both always gives us a copy of the whole thing.(this is the pythonic way to copy a sequence like a string or list)|
s[1:100]|'ello'|char starting at index 1 to the end of the string.|
s[-1] |'o'|last char(1st from the end)|
s[-4] |'e' |4th from the end.|
s[:-3] |'He' |going up to but not including the last 3 chars(exclude last 3 chars).|
s[-3:] |'llo'|starting with the 3rd char from the end and extending to the end of the string(last 3 char).|
s[::-1] | 'olleh' | Reverses the characters of the string. |
```python
s[:1] + s[1:] == s # True
```

slicing also works with three arguements. If the third argument is for example 3, only every third element from the range of the first two arguments will be taken.

```python
>>>str = "Python under Linux is great"
>>>str[1::3]
#finds every third string starting from the first
'youeLuiga'
```
