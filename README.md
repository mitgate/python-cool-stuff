# python-cool-stuff
- [x] Cool stuff in Python
- [x] You can test it in: https://paiza.io/en/projects/new?language=python3
- [x] The results are commented for you to copy and paste in your preferred interpreter
- [x] Yes, you can contribute with more ideas

 
# Mathematical division that rounds down to nearest integer.

The floor division operator is //.

For example, the expression 11 // 4 evaluates to 2 in contrast to the 2.75 returned by float true division.


- Python3:
```
print ( 11//4 )
# 2
print( 11/4 )
# 2.75
```
Note that (-11) // 4 is -3 because that is -2.75 rounded downward
```
print ( -11//4 )
# -3 
print ( -11/4 )
# -2.75 
```

- Python2:
```
print ( 11//4 )
# 2 
print ( 11/4 )
# 2 

print ( -11//4 )
# -3 
print ( -11/4 )
# -3 
```


# Combined multiply and assignment
```
somevar = '*' 
somevar *= 33
print(somevar)
# *********************************
```


# Some things Under the hood

The *= always calls __imul__ on the left hand operand :

```
product = [1] 
product *= 5
print ( product )
# [1, 1, 1, 1, 1]
```
is equivalent to :
```
product = [1] 
product.__imul__(5)
print ( product )
# [1, 1, 1, 1, 1]
```
