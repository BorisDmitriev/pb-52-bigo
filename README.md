# big-O-exercise

### Analyze the time complexity of the following functions. Which Big O classes do they each belong to? Also write a reason

#### foo
```javascript
const foo = array => {
  return array[0] * array[array.length - 1];
};

foo([3, 5, 1, 4, 7]); // 21
```
#### bar
```javascript
const bar = n => {
  while (n > 1) {
    console.log(n);
    n = n / 2;
  }
  console.log('done');
};

bar(32); // 32 16 8 4 2 done
```
#### boom
```javascript
const boom = n => {
  for (let q = 0; q < n; q++) {
    for (let r = 0; r < n; r++) {
      for (let s = 0; s < n; s++) {
        console.log(q, r, s);
      }
    }
  }
};

boom(2);
```
