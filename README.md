# Python-Exercise-Functions
This repository contains Python functions developed as exercises for a DevSecOps course.


### Practice Ideas

1. Create a function that receives a list of numbers and returns only elements that can be divided by 3.

### Answer to Exercise 1

```python
number_list = range(0, 1000)
list_of_three = [x for x in number_list if x % 3 == 0]
print(list_of_three)
```

Output:
```css
[0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 33, 36, 39, 42, 45, 48, 51, 54, 57, 60, 63, 66, 69, 72, 75, 78, 81, 84, 87, 90, 93, 96, 99, 102, 105, 108, 111, 114, 117, 120, 123, 126, 129, 132, 135, 138, 141, 144, 147, 150, 153, 156, 159, 162, 165, 168, 171, 174, 177, 180, 183, 186, 189, 192, 195, 198, 201, 204, 207, 210, 213, 216, 219, 222, 225, 228, 231, 234, 237, 240, 243, 246, 249, 252, 255, 258, 261, 264, 267, 270, 273, 276, 279, 282, 285, 288, 291, 294, 297, 300, 303, 306, 309, 312, 315, 318, 321, 324, 327, 330, 333, 336, 339, 342, 345, 348, 351, 354, 357, 360, 363, 366, 369, 372, 375, 378, 381, 384, 387, 390, 393, 396, 399, 402, 405, 408, 411, 414, 417, 420, 423, 426, 429, 432, 435, 438, 441, 444, 447, 450, 453, 456, 459, 462, 465, 468, 471, 474, 477, 480, 483, 486, 489, 492, 495, 498, 501, 504, 507, 510, 513, 516, 519, 522, 525, 528, 531, 534, 537, 540, 543, 546, 549, 552, 555, 558, 561, 564, 567, 570, 573, 576, 579, 582, 585, 588, 591, 594, 597, 600, 603, 606, 609, 612, 615, 618, 621, 624, 627, 630, 633, 636, 639, 642, 645, 648, 651, 654, 657, 660, 663, 666, 669, 672, 675, 678, 681, 684, 687, 690, 693, 696, 699, 702, 705, 708, 711, 714, 717, 720, 723, 726, 729, 732, 735, 738, 741, 744, 747, 750, 753, 756, 759, 762, 765, 768, 771, 774, 777, 780, 783, 786, 789, 792, 795, 798, 801, 804, 807, 810, 813, 816, 819, 822, 825, 828, 831, 834, 837, 840, 843, 846, 849, 852, 855, 858, 861, 864, 867, 870, 873, 876, 879, 882, 885, 888, 891, 894, 897, 900, 903, 906, 909, 912, 915, 918, 921, 924, 927, 930, 933, 936, 939, 942, 945, 948, 951, 954, 957, 960, 963, 966, 969, 972, 975, 978, 981, 984, 987, 990, 993, 996, 999]
```

2. Create a function that receives a list of numbers and does the following:
   - Print "fizz" if the number is divisible by 3.
   - Print "bazz" if the number is divisible by 6.
   - Print "buzz" if the number is divisible by 9.
   - Print "fizzbazzbuzz" if the number can be divided by all three preceding numbers.
   - In any other case, print the number itself.

### Answer to Exercise 2

```python
def filter_of_number(number_list):
    result = []
    for x in number_list:
        if x % 3 == 0 and x % 6 == 0 and x % 9 == 0:
            result.append("fizzbazzbuzz")
        elif x % 9 == 0:
            result.append("buzz")
        elif x % 6 == 0:
            result.append("bazz")
        elif x % 3 == 0:
            result.append("fizz")
        else:
            result.append(x)
    return result

my_number = range(0, 200)
my_result = filter_of_number(my_number)
print(my_result)
```

Output:

```css
['fizzbazzbuzz', 1, 2, 'fizz', 4, 5, 'bazz', 7, 8, 'buzz', 10, 11, 'bazz', 13, 14, 'fizz', 16, 17, 'fizzbazzbuzz', 19, 20, 'fizz', 22, 23, 'bazz', 25, 26, 'buzz', 28, 29, 'bazz', 31, 32, 'fizz', 34, 35, 'fizzbazzbuzz', 37, 38, 'fizz', 40, 41, 'bazz', 43, 44, 'buzz', 46, 47, 'bazz', 49, ...]
```

3. Create a function that can count the occurrences of a character within a given string. The function receives two parameters:
   - The character.
   - The string (which can also contain whitespaces).

### Answer to Exercise 3

```python
"I wish you a day full of joy and success.".count('a')
```
Output:

```css
3
```


