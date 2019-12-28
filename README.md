# KatasDelivery

## Numbers to letters

```
function switcher(x){
  const alphabet = ['z','y','x','w','v','u','t','s','r','q','p','o','n','m','l','k','j','i','h','g','f','e','d','c','b','a','!','?',' '];
  let word='';
  for (let i = 0; i < x.length; i++){
    if (x[i]<30){
      word += alphabet[x[i]-1];
    }
  }
  return word;
}
```

## Remove First and Last Character

```
function removeChar(str){
  if(str.length > 2){
    return str.slice(1, -1);
  }
  else{
    return str;
  }
}
```

## Vowel count

```
function getCount(str) {
  let vowelsCount = 0;
  for (let i = 0; i < str.length; i++) {
    if (str.charAt(i) == "a" || str.charAt(i) == "e" || str.charAt(i) == "i" || str.charAt(i) == "o" || str.charAt(i) == "u"){
      vowelsCount += 1;
    }
  }
  return vowelsCount;
}
```

## Sum Mixed Array

```
function sumMix (x){
  let sum = 0
  for(var i = 0; i < x.length; i++){
    const parsed = parseInt(x[i])
    sum += parsed;
  }
  return sum;
}
```

## Count of positives / sum of negatives

```
function countPositivesSumNegatives(input){
  let posCont = 0;
  let negSum = 0;
  if (input !== null){
    for(var i = 0; i < input.length; i++){
      if (input[i] <= 0){
        negSum += input[i];
      } else {
        posCont += 1;
      }
    }
  }
  return (input !==null && input.length > 0) ? [posCont, negSum] : [];
}
```

## Get the mean of an array

```
function getAverage(marks){
  let sum = 0;
  for(var i = 0; i < marks.length; i++){
    sum += marks[i];
  }
  return Math.floor(sum / marks.length);
}
```
