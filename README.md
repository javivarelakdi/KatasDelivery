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
    return str.slice(1, -1)
   }
   else{
   return str
   }
};
```
