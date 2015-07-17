Psuedocode
```
function removeVowels(string)
    tmpString = ''
    loop through each letter of the string
        if the letter is not a vowels
            add it to tmpString
    return tmpString
```

A Javascript solution
``` javascript
function removeVowels(str) {
    var tmpStr = '', vowels = ['a','e','i','o','u'];
    for (var i = 0; i <str.length; i++) {
        if (vowels.indexOf(str.charAt(i).toLowerCase()) === -1) //not a vowel
            tmpStr += str.charAt(i);
    }
    return tmpStr;
}
```

Python Solution

#Function removeVowels() - assumes String input
#search for each vowel (a,e,i,o,u) in the string 

def removeVowels(st):
	l= len(st)
	k= 0
	st1= ""
	while k<l:
		if st[k]== 'a' or st[k]== 'i' or st[k]== 'o' or st[k]== 'u' or st[k]== 'e':
			st1= st1
			k= k+1
		else:
			st1= st1 + st[k]
			k= k+1
	print(st1)
