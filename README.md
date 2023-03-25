# Quick Response Codes
While conventional bar codes are capable of storing a maximum of approximately 20 digits, QR Code is capable of handling several dozen to several hundred times more information.

QR Code is capable of handling all types of data, such as numeric and alphabetic characters, Kanji, Kana, Hiragana, symbols, binary, and control codes. Up to 7,089 characters can be encoded in one symbol.

# Content
Content is the text that needs to be send to the code reader. The text is normally an URL to a web site, or a code that is used by an application, for example in handling secrets in time based one time password applications.

# Size, padding and responsive
You can set the size used for generation, the larger the size, the more information you are able to store in the QR code. The size is also used for the container in pixels. You can also specify the padding in module units, and recommended minimum is 4.

With the repsponsive settings enabled, the size settings will only be used in the code calculation, and the container will addapt and use all available space in it's parent element.

# Colours
With the colour settings, you can control both the front and background colour.

## QR Code error correction
QR Code has error correction capability to restore data if the code is dirty or damaged. Four error correction levels are available for users to choose according to the operating environment. Raising this level improves error correction capability but also increases the amount of data QR Code size.
To select error correction level, various factors such as the operating environment and QR Code size need to be considered. Level Q or H may be selected for factory environment where QR Code get dirty, whereas Level L may be selected for clean environment with the large amount of data. Typically, Level M (15%) is most frequently selected.

Level L  Approx 7%
Level M  Approx 15%
Level Q  Approx 25%
Level H  Approx 30%




# create-svelte

Everything you need to build a Svelte library, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte).

Read more about creating a library [in the docs](https://kit.svelte.dev/docs/packaging).



## Building

To build your library:

```bash
npm run package
```

To create a production version of your showcase app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.

## Publishing

Go into the `package.json` and give your package the desired name through the `"name"` option. Also consider adding a `"license"` field and point it to a `LICENSE` file which you can create from a template (one popular option is the [MIT license](https://opensource.org/license/mit/)).

To publish your library to [npm](https://www.npmjs.com):

```bash
npm publish
```
