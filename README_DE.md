# big-O-exercise

### Analysiere die Zeit-Komplexität der folgenden Funktionen. Zu welchen Big O-Klassen gehören sie jeweils? Schreibe auch eine Begründung auf

#### foo
```javascript
const foo = array => {
  return array[0] * array[array.length - 1];
};

foo([3, 5, 1, 4, 7]); // 21
//O(1) Konstante Anzahl an Ausführungen unabhängig von der Eingabe




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
// O(log n) Die Anzahl der Ausführungen wird halbiert



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
// O(n^3)  => O(n^2) Die Anzahl der Ausführungen wird verdreifacht
```
