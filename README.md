In this exercise, we are using a points dictionary, with each character as a key in the alphabet corresponding to a numeric point assigned as the value for each key. 

Much like dict_pts.py, which contained a single variable as a string. This exercise has two major differences. One is that, we are using a list dataset of words in addition to using the dictionary dataset. The challenge is to be able to iterate via both datasets. Which we come to the second distinction of using a nested for loop. 

The first for loop is looping over the list dataset and the second for loop is looping over the substrings of each individual word. A conditional statement is used to compare the characters (char) against the char in the dictionary:

    if char in points:
        point += points[char]

The breakdown here is that for each char in the words variable, the total points should be based on the key to which each points are assigned its value. For example, if we assigned the word "Lay" to the word variable.

    word = "Lay"

Now we iterate over the word:
    for word in words:
        for char in word.lower():
            if char in points:
                point += points[char]

Lets evaluate how we total the points:
    point = Lay
    l = 12
    a = 1
    y = 25
    point = Lay
    Lay.lower() = lay
    point = l   +a  +y
    point = 12  +1  +25
    point = 38