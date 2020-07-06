# 📘What is Purebook

------

**PureBook** is a minimal and beauty themes for Typora. This theme is good for code and read.

Our mission is to make a **user-friendly** and **collaborative** product for everyone to create, edit and share knowledge through documentation.

------

## 🌠Features

- 👨‍💻‍ Code-Fences fonts use Cascadia Code. This fonts support ligature, when you enter code text same as ‘=>‘ then will be auto change  one character `=>`
- 💻

#### Code Fences

```javascript
class Utils {
  animate(element: Element, attr: string, change: { from: number, to: number, duration?: number }, onEnd?: () => void) {
    if (change.from = = change.to) return;

    if (!change.duration)
      element[attr] = change.to;

    const easing = (t, b, c, d) => c * ((t = t / d - 1) * t * t + 1) + b,
      { from, to } = change,
      during = Math.ceil((change.duration || 300) / 17) || 1;

    let start = 0,
      instance = null;

    step();

    function step() {
      const value = Math.ceil(easing(start, from, to - from, during));

      start++;
      if (start <= during) {
        element[attr] = value;
        instance = requestAnimationFrame(step);
      }
      else {
        if (onEnd) onEnd();
        cancelAnimationFrame(instance);
      }
    }
  }
}
```



[this is a url](https://www.google.com)

