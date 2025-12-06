#1- 
to find the sum of 2 numbers (num1+num2)

class Solution:
    def sum(self, num1: int, num2: int) -> int:
        return num1+num2

t.c: O(1)
s.c: O(1)

#2
-to find whether the sum of left nd right nodes equals the parent node.. (only contains 3 nodes total)

class Solution:
    def checkTree(self, root):
        return root.val == root.left.val+ root.right.val

t.c: O(1)
s.c: O(1)

#3- to add the consecutive int. value in a list nd returning those added n listed values .OR. running sum of 1d array.

class Solution:
    def runningSum(self, nums: List[int]) -> List[int]:
       for i in range(1,len(nums)):
           nums[i]=nums[i-1]+ nums[i]       # OR-> nums[i]+=nums[i-1]
       return nums

# Alt solution:
class Solution:
 def runningSum(self, nums: List[int]) -> List[int]:
   return [sum(nums[:i+1]) for i in range(len(nums))]

t.c: O(n)
s.c: O(1)

#4- to find the maximum wealth in the accs of bank's customers

class Solution:
    def maximumWealth(self, accounts: List[List[int]]) -> int:
        rich=0
        for i in accounts:
            rich=max(rich,sum(i))
        return rich
t.c: O(n*m)
s.c: O(1)


#5- to do the fizz, buzz, fizzbuzz game with multiples of 3, 5, nd 3&5(15) respectively

class Solution:
    def fizzBuzz(self, n: int) -> List[str]:
        a=[]
        for i in range(1,n+1):
            if i%15==0:
                a.append("FizzBuzz")
            elif i%5==0:
                a.append("Buzz")
            elif i%3==0:
                a.append("Fizz")
            else:
                a.append(str(i))
        return a

t.c= O(n)
s.c= O(n)

#6- 

#7-

#8-


*t.c- time complexity
*s.c- space complexity

practice sesh:
#1:
class Solution:
  def sum(self, num1:int, num2:int)-> int:
      return num1+num2

