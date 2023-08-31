```python
temp = [20, 25, 30, 34, 32, 36, 35, 31, 35, 37, 33, 38, 35
              , 26, 28, 29, 23, 22, 24, 27] # list of human tempratures

temp.sort() # re-arranging temp 
mean = sum(temp)/len(temp) 
print("The mean is ==>", round(mean,2)) # getting result 
```

    The mean is ==> 30.0
    


```python
if len(temp) % 2 == 1: # identifying if the lenght of the list obeject is odd or even
    median = temp[len(temp) // 2] # printing the output when lenght is odd  
else:
    middle1 = temp[len(temp) // 2 - 1]
    middle2 = temp[len(temp) // 2]
    median = (middle1 + middle2) / 2
    
print("sorted_temp ==>", temp)
print("Median temperature:", median) # getting result
```

    sorted_temp ==> [20, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 35, 35, 36, 37, 38]
    Median temperature: 30.5
    


```python
# Calculate squared differences for variance
squared_diff = [(x - mean) ** 2 for x in temp]

# Calculate variance
variance = sum(squared_diff) / len(temp)

# Calculate standard deviation
std_dev = variance ** 0.5

# Calculate standard deviation
temp_range = max(temp) - min(temp)

# getting result
print("Temprature range ==>", temp_range)
print("Variance of the list object is ==>", round(variance,2))
print("Standard deviation of the list obeject ==>",round(std_dev,2))
```

    Temprature range ==> 18
    Variance of the list object is ==> 27.9
    Standard deviation of the list obeject ==> 5.28
    


```python

```
