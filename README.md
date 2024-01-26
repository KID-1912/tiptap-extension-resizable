# tiptap-extension-resizable

<h3 align="center">
    This is a Tiptap extension designed to enable resizing for your Tiptap content, including elements such as images and videos
</h3>

<br/>

<p align="center">
  <a href="https://www.npmjs.com/package/tiptap-extension-resizable">
    <img
     alt="NPM URL"
     src="https://img.shields.io/badge/npm-tiptapExtensionResizable?logo=npm">
  </a>
  <img
     alt="version"
     src="https://img.shields.io/badge/version-1.1.1-blue">
</p>

[![](https://raw.githubusercontent.com/KID-1912/Github-PicGo-Images/master/202312101313640.png)](https://www.npmjs.com/package/tiptap-extension-resizable)

<br>

---

## Tnstall

```shell
npm install tiptap-extension-resizable -S
```

## Usage

```js
import Resizable from "tiptap-extension-resizable";

const editor = new Editor({
  element: document.querySelector(".editor"),
  extensions: [StarterKit, Image.configure({ inline: true }), Resizable],
});
```

## Options

You can configure extension options, which are optional.

```js
  extensions: [
    StarterKit,
    Image.configure({ inline: true }),
    Resizable.configure({
      types: ["image", "video"], // resizable type
      handlerStyle: { // handler point style
        width: "8px",
        height: "8px",
        background: "#07c160",
      },
      layerStyle: { // layer mask style
        border: "2px solid #07c160",
      },
    }),
  ],
```

## Relations

**@tiptap/extension-image:** https://github.com/ueberdosis/tiptap/tree/develop/packages/extension-image

**tiptap-appmsg-editor:** https://github.com/KID-1912/tiptap-appmsg-editor
