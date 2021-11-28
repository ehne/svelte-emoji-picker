<h1 align="center">Welcome to svelte-emoji-picker 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
  <a href="https://twitter.com/coolbezos">
    <img alt="Twitter: coolbezos" src="https://img.shields.io/twitter/follow/coolbezos.svg?style=social" target="_blank" />
  </a>
</p>

> A simple emoji picker component for Svelte

## Demo
A demo can be found [here](https://svelte.dev/repl/9afc56aabfff4382883278dbdf4ce9fd?version=3.8.1)

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
|emojis| [Emoji Array](https://github.com/ehne/svelte-emoji-picker/blob/master/src/index.svelte) | An array of the emojis that the user can select from |
|fontSize | "30px" | the font size of the emojis|


## Author

* Github: [@ehne](https://github.com/ehne)

## Show your support

Give a ⭐️ if this project helped you!

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
