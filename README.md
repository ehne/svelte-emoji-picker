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
|emojis| ![Emoji Array](https://og.darcylf.me/%5B%22%E2%9C%8C%EF%B8%8F%22%2C%22%F0%9F%98%82%22%2C%22%F0%9F%98%9D%22%2C%22%F0%9F%98%81%22%2C%22%F0%9F%98%B1%22%2C%22%F0%9F%91%89%22%2C%22%F0%9F%99%8C%22%2C%22%F0%9F%8D%BB%22%2C%22%F0%9F%94%A5%22%2C%22%F0%9F%8C%88%22%2C%22%E2%98%80%EF%B8%8F%22%2C%22%F0%9F%8E%88%22%2C%22%F0%9F%8C%B9%22%2C%22%F0%9F%92%84%22%2C%22%F0%9F%8E%80%22%2C%22%E2%9A%BD%22%2C%22%F0%9F%8E%BE%22%2C%22%F0%9F%8F%81%22%2C%22%F0%9F%98%A1%22%2C%22%F0%9F%91%BF%22%2C%22%F0%9F%90%BB%22%2C%22%F0%9F%90%B6%22%2C%22%F0%9F%90%AC%22%2C%22%F0%9F%90%9F%22%2C%22%F0%9F%8D%80%22%2C%22%F0%9F%91%80%22%2C%22%F0%9F%9A%97%22%2C%22%F0%9F%8D%8E%22%2C%22%F0%9F%92%9D%22%2C%22%F0%9F%92%99%22%2C%22%F0%9F%91%8C%22%2C%22%E2%9D%A4%22%2C%22%F0%9F%98%8D%22%2C%22%F0%9F%98%89%22%2C%22%F0%9F%98%93%22%2C%22%F0%9F%98%B3%22%2C%22%F0%9F%92%AA%22%2C%22%F0%9F%92%A9%22%2C%22%F0%9F%8D%B8%22%2C%22%F0%9F%94%91%22%2C%22%F0%9F%92%96%22%2C%22%F0%9F%8C%9F%22%2C%22%F0%9F%8E%89%22%2C%22%F0%9F%8C%BA%22%2C%22%F0%9F%8E%B6%22%2C%22%F0%9F%91%A0%22%2C%22%F0%9F%8F%88%22%2C%22%E2%9A%BE%22%2C%22%F0%9F%8F%86%22%2C%22%F0%9F%91%BD%22%2C%22%F0%9F%92%80%22%2C%22%F0%9F%90%B5%22%2C%22%F0%9F%90%AE%22%2C%22%F0%9F%90%A9%22%2C%22%F0%9F%90%8E%22%2C%22%F0%9F%92%A3%22%2C%22%F0%9F%91%83%22%2C%22%F0%9F%91%82%22%2C%22%F0%9F%8D%93%22%2C%22%F0%9F%92%98%22%2C%22%F0%9F%92%9C%22%2C%22%F0%9F%91%8A%22%2C%22%F0%9F%92%8B%22%2C%22%F0%9F%98%98%22%2C%22%F0%9F%98%9C%22%2C%22%F0%9F%98%B5%22%2C%22%F0%9F%99%8F%22%2C%22%F0%9F%91%8B%22%2C%22%F0%9F%9A%BD%22%2C%22%F0%9F%92%83%22%2C%22%F0%9F%92%8E%22%2C%22%F0%9F%9A%80%22%2C%22%F0%9F%8C%99%22%2C%22%F0%9F%8E%81%22%2C%22%E2%9B%84%22%2C%22%F0%9F%8C%8A%22%2C%22%E2%9B%B5%22%2C%22%F0%9F%8F%80%22%2C%22%F0%9F%8E%B1%22%2C%22%F0%9F%92%B0%22%2C%22%F0%9F%91%B6%22%2C%22%F0%9F%91%B8%22%2C%22%F0%9F%90%B0%22%2C%22%F0%9F%90%B7%22%2C%22%F0%9F%90%8D%22%2C%22%F0%9F%90%AB%22%2C%22%F0%9F%94%AB%22%2C%22%F0%9F%91%84%22%2C%22%F0%9F%9A%B2%22%2C%22%F0%9F%8D%89%22%2C%22%F0%9F%92%9B%22%2C%22%F0%9F%92%9A%22%5D.png?theme=light&md=1&fontSize=50px&images=https%3A%2F%2Fcdn.darcylf.me%2Fdarcy_badge%2Fcircle-on-white.svg&heights=200 "The Array Of Emojis")| An array of the emojis that the user can select from |
|fontSize | "30px" | the font size of the emojis|


## Author

👤 **Darcy Lugt-Falk**

* Twitter: [@coolbezos](https://twitter.com/coolbezos)
* Github: [@ehne](https://github.com/ehne)

## Show your support

Give a ⭐️ if this project helped you!

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_