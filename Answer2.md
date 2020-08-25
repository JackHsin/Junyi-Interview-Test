# Answer
第一直覺是想從頭到尾一個一個數字去除以3,5和15做數量增減。但覺得太慢。

想想覺得透過除法和倍數的概念應該可以更快解答，將input的數字除以3,5,15得到的結果就是input裡面倍數的個數，之後只要將3, 5的都扣掉，在把15的加回來兩次就可以了。

JavaScript
```javascript
const filter_3_5_but_15 = input => {
  let three_out = Math.floor(input / 3);
  let five_out = Math.floor(input / 5);
  let fifteen_out = Math.floor(input / 15);
  return input + (fifteen_out * 2) - three_out - five_out; 
}

filter_3_5_but_15(15)
9
filter_3_5_but_15(30)
18
filter_3_5_but_15(100)
59
filter_3_5_but_15(1500)
900
```
