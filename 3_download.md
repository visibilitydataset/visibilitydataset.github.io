---
sort: 3
---

# Request Downloads

```note
This is note2
```

`inline code`

```
:root {
  @for $level from 1 through 12 {
    @if $level % 4 == 0 {
      --toc-#{$level}: #{darken($theme-white, 4 * 8.8%)};
    } @else {
      --toc-#{$level}: #{darken($theme-white, $level % 4 * 8.8%)};
    }
  }
}
```

I give this theme two :+1:!

```tip
Set config `plugins: [jemoji]`, Emoji searcher, see: [https://emoji.muan.co/](https://emoji.muan.co/)
```
Text can be **bold**, _italic_, or ~~strikethrough~~. [Links](https://github.com) should be blue with no underlines (unless hovered over).
