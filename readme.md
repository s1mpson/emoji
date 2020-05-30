# emoji ![GitHub](https://img.shields.io/github/license/s1mpson/emoji)

> Simple emoji support for [Deno](https://deno.land/) (validate, detect, trim, extract)

### Contents
- [`Import`](#import)
- [`Methods`](#methods)
  - [`isEmoji`](#isemoji-string)
  - [`hasEmoji`](#hasemoji-string)
  - [`trimEmoji`](#trimemoji-string)
  - [`extractEmoji`](#extractemoji-string)
- [`Licence`](#license)

### Import

```ts
import { isEmoji } from "https://raw.githubusercontent.com/s1mpson/emoji/master/mod.ts";
```

## Methods

### isEmoji (string)

Returns **true** if provided string is a valid emoji.

```ts
isEmoji('🤔'); // true
isEmoji('?'); // false
```

### hasEmoji (string)

Returns **true** if there is at least one emoji in string.

```ts
hasEmoji('Sadly, no unicorns found..'); // false
hasEmoji('But we have one here: 🦄'); // true
```

### trimEmoji (string)

Returns the string cleaned from emoji.

```ts
trimEmoji('Just 👏 Do 👏 It'); // "Just  Do  It"
```

### extractEmoji (string)

Returns an array of emoji extracted from the string.

```ts
extractEmoji('🦕 ❤️ 🦄'); // ["🦕", "❤️", "🦄"]
```

## License
Copyright © [Max Mikhalchuk](https://github.com/s1mpson).
Licensed under the [MIT License](https://github.com/s1mpson/emoji/blob/master/license).