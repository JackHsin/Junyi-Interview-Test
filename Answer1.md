# Answer
Q1.1 使用javascript基本的split, reverse, join完成字串反轉處理。

Q1.2 使用第一題的reverseString function去處理句子split後的單字，再重新join回來。
```javascript
// Q1.1
const string = "junyiacademy"
const reverseString = string => string.split("").reverse().join("")

reverseString(string)
"ymedacaiynuj"

// Q1.2
const sentence = "flipped class room is important"
const reverseStringInSentence = sentence => sentence.split(" ").map( string => reverseString (string) ).join(" ")

reverseStringInSentence(sentence)
"deppilf ssalc moor si tnatropmi"
````
