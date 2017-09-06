### ログに色をつける
```javascript
console.log('%cHello %cWorld', 'color: red;', 'background-color: black; color: cyan; font-weight: bold;');
```

## オブジェクトを表示する

```javascript
const obj = { hoge: 'fuga', piyo: 'moge' };
console.group('%c[DEBUG] %ctitle', 'background-color: black; color: cyan;', 'font-weight: bold; font-style:italic');
console.log(obj);
console.groupEnd();
```

## タイムスタンプを表示する

```javascript
const pad = (num, maxLength) => {
  return '0'.repeat(maxLength - num.toString().length) + num;
};

const timestamp = () => {
  const time = new Date();
  return '@ ' +
    pad(time.getHours(), 2) + ':' +
    pad(time.getMinutes(), 2) + ':' +
    pad(time.getSeconds(), 2) + '.' +
    pad(time.getMilliseconds(), 3);
}

console.log('%choge', 'color: red', timestamp());
```

