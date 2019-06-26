# Codewars Katas Solved since 06.25.19
_________________


| Name          | Link          | Date     |
| ------------- |:-------------:| :-------:|
| Who is going to pay for the wall?  |[https://www.codewars.com/kata//58bf9bd943fadb2a980000a7](https://www.codewars.com/kata//58bf9bd943fadb2a980000a7 "Who is going to pay for the wall?") | 06.25.19 |
| Sum Mixed Array   |[https://www.codewars.com/kata//57eaeb9578748ff92a000009](https://www.codewars.com/kata//57eaeb9578748ff92a000009 "Sum Mixed Array")     | 06.25.19 |
| Multiples of 3 or 5 |[https://www.codewars.com/kata//514b92a657cdc65150000006](https://www.codewars.com/kata//514b92a657cdc65150000006 "Multiples of 3 or 5")       | 06.25.19 |
| Count Odd Numbers below n  |[https://www.codewars.com/kata//59342039eb450e39970000a6](https://www.codewars.com/kata//59342039eb450e39970000a6 "Count Odd Numbers below n")        | 06.25.19 |
| Array plus array |[https://www.codewars.com/kata/5a2be17aee1aaefe2a000151](https://www.codewars.com/kata/5a2be17aee1aaefe2a000151 "Array plus array")      | 06.25.19 |


# My Solutions
________________
## Initial Level
### 06.25.19

**Who is going to pay for the wall?**  [https://www.codewars.com/kata//58bf9bd943fadb2a980000a7](https://www.codewars.com/kata//58bf9bd943fadb2a980000a7 "Who is going to pay for the wall?")
```javascript
function whoIsPaying(name){
  let arr = [name];
  if (name.length > 2){
  let name2 = name.substring(0,2)
  arr.push(name2);
  }
  return arr;
}
```

**Sum Mixed Array**  [https://www.codewars.com/kata//57eaeb9578748ff92a000009](https://www.codewars.com/kata//57eaeb9578748ff92a000009 "Sum Mixed Array")
```javascript
function sumMix(x){
  let sum = 0;
  for ( let i = 0; i < x.length; i++){
    if(typeof x[i] === 'string'){
      x[i] = Number(x[i]);
    }
    sum += x[i];
  }
  return sum;
}
```

**Multiples of 3 or 5**  [https://www.codewars.com/kata//514b92a657cdc65150000006](https://www.codewars.com/kata//514b92a657cdc65150000006 "Multiples of 3 or 5")
```javascript
function solution(number){
  let sum = 0;
  for (i = 3; i < number; i++){
    if( i % 3 === 0 || i % 5 === 0){
      sum += i;
    }
  }
  return sum;
}
```

**Count Odd Numbers below n**  [https://www.codewars.com/kata//59342039eb450e39970000a6](https://www.codewars.com/kata//59342039eb450e39970000a6 "Count Odd Numbers below n")
```javascript
function oddCount(n){
  return Math.floor(n / 2);
}
```

**Array plus array**  [https://www.codewars.com/kata/5a2be17aee1aaefe2a000151](https://www.codewars.com/kata/5a2be17aee1aaefe2a000151 "Array plus array")
```javascript
function arrayPlusArray(arr1, arr2) {
  let arrSum = 0;
  for (let i = 0; i < arr1.length; i++){
    arrSum += arr1[i];
  }
  for (let i = 0; i < arr2.length; i++){
    arrSum += arr2[i];
  }
  return arrSum;
}
```
