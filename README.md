<h1 align="center">Welcome to svelte-emoji-picker 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
  <a href="https://twitter.com/coolbezos">
    <img alt="Twitter: coolbezos" src="https://img.shields.io/twitter/follow/coolbezos.svg?style=social" target="_blank" />
  </a>
</p>

> A simple emoji picker component for Svelte

## Install
```bash
npm i svelte-emoji-picker
```

## Usage
```html
<!-- App.svelte -->
<script>
    import EmojiPicker from 'svelte-emoji-picker';
    let text
</script>

<textarea bind:value={text}></textarea>
<EmojiPicker bind:value={text} />

```

### Props

| prop | default value | description
|-|-|-|
|emojis| ![Emoji Array](./emojiList.png "The Array Of Emojis")| An array of the emojis that the user can select from |
|fontSize | "30px" | the font size of the emojis|


## Author

👤 **Darcy Lugt-Falk**

* Twitter: [@coolbezos](https://twitter.com/coolbezos)
* Github: [@ehne](https://github.com/ehne)

## Show your support

Give a ⭐️ if this project helped you!

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_