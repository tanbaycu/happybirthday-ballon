# 🎉 Interactive Birthday Animation
*made by tanbaycu*

Welcome to the Interactive Birthday Animation project! This vibrant, canvas-based animation brings birthday wishes to life with dazzling fireworks and floating balloons.

[![Demo](https://i.postimg.cc/gkF836qH/chrome-qiuv-R8-M27-V.gif)](https://postimg.cc/Dm6ST0NS)

## 🌟 Features

- Dynamic text animation with customizable messages
- Firework effects with realistic physics
- Balloon animations with natural floating behavior
- Responsive design that adapts to various screen sizes

## 🎨 Customization

Personalize your birthday message by modifying the `opts` object in `happy birtday.js`:

```javascript
opts = {
  strings: ["HAPPY", "BIRTHDAY!", "to You"],
  // ... other options
}
```

Adjust other parameters like colors, sizes, and animation timings to create your perfect birthday spectacle!

## 🚀 Performance Tips

- The animation is optimized for smooth performance, but on lower-end devices, you may want to reduce the number of particles or animation complexity.
- Use the `opts.fireworkBaseShards` and `opts.fireworkAddedShards` to control the number of firework particles.

## 🔧 Advanced Usage

### Creating Custom Shapes

Extend the `generateBalloonPath` function to create your own custom shapes:

```javascript
function generateCustomShape(x, y, size) {
  ctx.beginPath();
  // Your custom shape drawing code here
  ctx.closePath();
}
```

### Adding Sound Effects

Enhance the experience with audio:

```javascript
const audio = new Audio('path/to/firework-sound.mp3');
// Play sound in the firework phase
if (this.phase === 'firework' && this.tick === this.reachTime) {
  audio.play();
}
```



## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.



---

Crafted with ❤️ and JavaScript magic. Happy Coding!