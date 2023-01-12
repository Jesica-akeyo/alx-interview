# 0x02. Minimum Operations
## Task 0 - Minimum operations

In a text file there is a single character`H`. Your text editor can execute two operations in this file: `Copy All` and `Paste`. Given the numver `n`, write a method that calcukates the fewest number of operations needed to result in exactly `n``H`characters in the file.

* Prototypke: `def minOperations(n)
* Returns an integer
* If `n` is impossile to achieve , return `0`

### Example:

`n = 9`

`H => Copy All => Paste => HH => Paste =>HHH => Copy All => Paste => HHHHHH => Paste => HHHHHHHHH`

Number of operations: `6`

```
carrie@ubuntu:~/0x02-minoperations$ cat 0-main.py
#!/usr/bin/python3
"""
Main file for testing
"""

minOperations = __import__('0-minoperations').minOperations

n = 4
print("Min # of operations to reach {} char: {}".format(n, minOperations(n)))

n = 12
print("Min # of operations to reach {} char: {}".format(n, minOperations(n)))

carrie@ubuntu:~/0x02-minoperations$
```

```
carrie@ubuntu:~/0x02-minoperations$ ./0-main.py
Min number of operations to reach 4 characters: 4
Min number of operations to reach 12 characters: 7
carrie@ubuntu:~/0x02-minoperations$
```
