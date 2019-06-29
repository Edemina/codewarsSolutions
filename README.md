# Codewars Katas Solved since 06.25.19
_________________


| Name          | Link          | Date     |
| ------------- |:-------------:| :-------:|
| Create Phone Number |[https://www.codewars.com/kata//525f50e3b73515a6db000b83](https://www.codewars.com/kata//525f50e3b73515a6db000b83 "Create Phone Number")      | 06.28.19 |
| Credit card issuer checking |[https://www.codewars.com/kata//5701e43f86306a615c001868](https://www.codewars.com/kata//5701e43f86306a615c001868 "Credit card issuer checking")      | 06.28.19 |
| Returning Strings |[https://www.codewars.com/kata//55a70521798b14d4750000a4](https://www.codewars.com/kata//55a70521798b14d4750000a4 "Returning Strings")      | 06.27.19 |
| pick a set of first elements |[https://www.codewars.com/kata//572b77262bedd351e9000076](https://www.codewars.com/kata//572b77262bedd351e9000076 "pick a set of first elements") | 06.26.19 |
| Jenny's secret message |[https://www.codewars.com/kata//55225023e1be1ec8bc000390](https://www.codewars.com/kata//55225023e1be1ec8bc000390 "Jenny's secret message") | 06.26.19 |
| Who is going to pay for the wall?  |[https://www.codewars.com/kata//58bf9bd943fadb2a980000a7](https://www.codewars.com/kata//58bf9bd943fadb2a980000a7 "Who is going to pay for the wall?") | 06.25.19 |
| Sum Mixed Array   |[https://www.codewars.com/kata//57eaeb9578748ff92a000009](https://www.codewars.com/kata//57eaeb9578748ff92a000009 "Sum Mixed Array")     | 06.25.19 |
| Multiples of 3 or 5 |[https://www.codewars.com/kata//514b92a657cdc65150000006](https://www.codewars.com/kata//514b92a657cdc65150000006 "Multiples of 3 or 5")       | 06.25.19 |
| Count Odd Numbers below n  |[https://www.codewars.com/kata//59342039eb450e39970000a6](https://www.codewars.com/kata//59342039eb450e39970000a6 "Count Odd Numbers below n")        | 06.25.19 |
| Array plus array |[https://www.codewars.com/kata/5a2be17aee1aaefe2a000151](https://www.codewars.com/kata/5a2be17aee1aaefe2a000151 "Array plus array")      | 06.25.19 |


# My Solutions_MASTER
________________
## Strings

**new solution +++++++++++++**

### 06.28.19

**Create Phone Number**  [[https://www.codewars.com/kata//525f50e3b73515a6db000b83](https://www.codewars.com/kata//525f50e3b73515a6db000b83 "Create Phone Number")
```javascript
function createPhoneNumber(n){
  let str1 = n.slice(0,3).join('');
  let str2 = n.slice(3,6).join('');
  let str3 = n.slice(6,10).join('');
  let str = `(${str1}) ${str2}-${str3}`;
  return str;
}
```

**Credit card issuer checking**  [https://www.codewars.com/kata//5701e43f86306a615c001868](https://www.codewars.com/kata//5701e43f86306a615c001868 "Credit card issuer checking")
```javascript
function getIssuer(number) {
  let n = number.toString();
   if (n.length == 15 && (n.substr(0, 2) === '34' || n.substr(0, 2) === '37')) return 'AMEX';
   if (n.length == 16 && n.substr(0, 4) === '6011') return 'Discover';
   if (n.length == 16 && (+n.substr(0, 2) >= 51  && +n.substr(0, 2) <= 55)) return 'Mastercard';
   if ((n.length === 13 || n.length === 16) && n.substr(0, 1) === '4') return 'VISA';
   return 'Unknown';
}
```

### 06.27.19

**Returning Strings**  [https://www.codewars.com/kata//55a70521798b14d4750000a4](https://www.codewars.com/kata//55a70521798b14d4750000a4 "Returning Strings")
```javascript
function first(arr, n=1) {
   return arr.slice(0,n);
}
```

## Initial Level

### 06.26.19

**pick a set of first elements**  [https://www.codewars.com/kata//572b77262bedd351e9000076](https://https://www.codewars.com/kata//572b77262bedd351e9000076 "pick a set of first elements")
```javascript
function first(arr, n=1) {
   return arr.slice(0,n);
}
```

**Jenny's secret message**  [https://www.codewars.com/kata//55225023e1be1ec8bc000390](https://www.codewars.com/kata//55225023e1be1ec8bc000390 "Jenny's secret message")
```javascript
function greet(name){
  return name === "Johnny" ? "Hello, my love!" : "Hello, " + name + "!";
}
```

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
