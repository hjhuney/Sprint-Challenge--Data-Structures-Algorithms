Add your answers to the Algorithms exercises here.

Exercise I
(a) O(1)
(b) O(1)
(c) O(n^3)
(d) O(n^2)
(e) O(n^3)
(f) O(n)
(g) O(n)


Exercise II
(a) 
array = [19,66,26,6,64]

def max_value(list):
  min = sorted(list)[0]
  max = sorted(list, reverse=True)[0]
  
  for i in list:
    if i < min:
      min = i
    if i > max:
      max = i
      
  return max - min

print(max_value(array))

(b) 
n = 30
f = 12

def egg_toss(n):
  toss_f = n // 2
  
  while toss_f != f:
    print(toss_f)
    if toss_f > f:
      toss_f = toss_f // 2
    elif toss_f < f:
      toss_f = toss_f + round((((toss_f * 2) - toss_f) / 2))
  return toss_f

egg_toss(30)


Exercise III
(a) O(n). While the array is sorted, the function still continues a for loop that iterates through every element in the array. 
(b) O(n). The same as above. To find the median, we have to search every element in the array. 
