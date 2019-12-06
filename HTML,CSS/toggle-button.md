# やりたいこと
こういうの
![toggle](https://user-images.githubusercontent.com/3584135/70301160-868a7700-17f1-11ea-9885-94801443d9e8.gif)

# やってみた
```html
<div class="toggle-button">
  <input type="checkbox" class="toggle" id="toggle" />
  <label for="toggle"></label>
</div>
```
```scss
.toggle-button {
  position: relative;
  width: 50px;
  height: 30px;

  input.toggle {
    position: absolute;
    left: 0;
    top: 0;
    cursor: pointer;
    opacity: 0;

    &:checked + label {
      background-color: #44db5e;
      border: 2px solid #44db5e;

      &:after {
        left: 20px;
      }
    }
  }

  label {
    width: 50px;
    height: 30px;
    background-color: #fff;
    border: 2px solid #e6e6e6;
    position: relative;
    display: inline-block;
    border-radius: 15px;
    transition: 0.4s;
    box-sizing: border-box;

    &:after {
      content: "";
      position: absolute;
      width: 26px;
      height: 26px;
      border-radius: 100%;
      left: 0;
      top: 0;
      background-color: #fff;
      box-shadow: 0 3px 3px rgba(0, 0, 0, 0.05), 0 2px 2px rgba(0, 0, 0, 0.1), 0 3px 1px rgba(0, 0, 0, 0.05);
      transition: 0.4s;
    }
  }
}
```

# コード
https://codepen.io/k-tada/pen/xxbGoJg
