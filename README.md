# Arrange-Alphabetical
Function that returns the string arranged alphabetically.

def arrange(s):
    new_s = ""
    #b = ""
    for i in s:
        b = i
        for j in range(len(new_s)):
           
            if ord(i) < ord(new_s[j]):
                new_s = new_s[:j] +b +new_s[j:]
                b = ""
        new_s += b

    return new_s  

