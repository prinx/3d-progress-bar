# A 3D Progress Bar

![Image](https://github.com/user-attachments/assets/7d119dc7-1097-4167-989b-cf42b04861d3)

## HTML

```html
<div class="progress-container">
  <div class="progress" style="width: 75%;"></div>
</div>
```

## CSS

```css
.progress-container {
  position: relative;
  width: 70%;
  height: 10%;
  border-radius: 9999px;
  background-color: rgba(200, 200, 200, 0.5);
}
.progress {
  height: 100%;
  border-radius: 9999px;
  position: absolute;
  background: radial-gradient(circle at 100% 100%, rgba(50, 150, 0, 1), rgb(50 150 0 / 80%) 60%, rgba(50, 150, 0, 0.7));
  transition: width 0.2s ease-in-out;
}
.progress:before {
  content: "";
  position: absolute;
  top: 30%;
  left: 8%;
  width: 90%;
  height: 20%;
  border-radius: 9999px;
  -webkit-filter: blur(1px);
  filter: blur(1px);
  background: radial-gradient(circle at 100% 100%, rgba(255, 255, 255, 0.4) 0, rgba(255, 255, 255, 0.3) 50%, rgba(255, 255, 255, 0.1) 100%);
}
```

You can also check this on [CodePen](https://codepen.io/prinx/pen/VwJGOay).

## License

[MIT](LICENSE)
