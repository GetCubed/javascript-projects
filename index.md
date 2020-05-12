# Welcome. This blog is about getting back to basics.

Enjoy this showcase series of Javascript based projects using just HTML, CSS, and Javascript. No **libraries**, no **frameworks**, and no **boilerplates**.

## Drum Kit

[**Check it out here**](./drum-kit/index.html)

use an `<audio>` tag to referece a wav file

```html
<audio data-key="65" src="sounds/clap.wav"></audio>
```

create the keys on the screen with a `<kbd>` tag

```html
<kbd>A</kbd> <span class="sound">clap</span>
```

then the script file

```javascript
const keys = document.querySelectorAll('.key');

keys.forEach((key) => {
    key.addEventListener('transitionend', (e) => {
        if (e.propertyName !== 'transform') return;
        e.target.classList.remove('playing');
    });
});

window.addEventListener('keydown', (e) => {
    const audio = document.querySelector(`audio[data-key="${e.keyCode}"]`);
    const key = document.querySelector(`div[data-key="${e.keyCode}"]`);
    if (!audio) return;

    audio.currentTime = 0;
    audio.play();

    key.classList.add('playing');
});
```
