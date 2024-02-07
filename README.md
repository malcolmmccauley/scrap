scrap
=====

Python - FizzBuzz

Given integer n, for each integer i in range from 1 to n inclusive print one value per line according to the following rules:

If i is a multiple of 3 and 5 print FizzBuzz
If i is a multiple of 3 print Fizz
If i is a multiple of 5 print Buzz
If i is a not multiple of 3 or 5 print the value of i

```python
def fizzBuzz(n):
    number = 1
    while number <= n:
        if number % 3 == 0 and number % 5 == 0:
            print('FizzBuzz')
        elif number % 3 == 0:
            print('Fizz')
        elif number % 5 == 0:
            print('Buzz')
        else:
            print(f'{number}')
        number += 1

if __name__ == '__main__':
    n = int(input().strip())

    fizzBuzz(n)
```

Two-Sums

With an integer array and an integer target, return indices of the two numbers such that they add up to target. Assume exactly one solution, and that the same element cannot be used twice.

```python
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        
        for index, number in enumerate(nums):
            for second_index, second_number in enumerate(nums):
                if index == second_index:
                    continue
                elif number + second_number == target:
                    return [index,second_index]
```
