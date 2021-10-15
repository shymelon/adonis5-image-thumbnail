<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Table of contents

- [adonis5-image-thumbnail](#adonis5-image-thumbnail)
  - [Installation](#installation)
  - [Usage](#usage)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# adonis5-image-thumbnail
> AdonisJS 5, image-thumbnail

 [![npm-image]][npm-url] [![license-image]][license-url] [![typescript-image]][typescript-url]

[Image thumbnail](https://github.com/onildoaguiar/image-thumbnail) provider for AdonisJS

## Installation
```bash
npm i --save adonis5-image-thumbnail
```

Compile your code:
```bash
node ace serve --watch
```
Connect all dependences:
```bash
node ace invoke adonis5-image-thumbnail
```
## Usage
After adding provider to your app, 
you can import ImageThumbnail to access its functions
```typescript
    const image = request.file('image')
    const thumbnail = await imageThumbnail(image.tmpPath,{width:150, height:150, withMetaData: true, fit: 'inside'})
```
For other options, please look at official library [documentation](https://github.com/onildoaguiar/image-thumbnail#readme)

[npm-image]: https://img.shields.io/npm/v/adonis5-image-thumbnail.svg?style=for-the-badge&logo=npm
[npm-url]: https://npmjs.org/package/adonis5-image-thumbnail "npm"

[license-image]: https://img.shields.io/npm/l/adonis5-image-thumbnail?color=blueviolet&style=for-the-badge
[license-url]: LICENSE.md "license"

[typescript-image]: https://img.shields.io/badge/Typescript-294E80.svg?style=for-the-badge&logo=typescript
[typescript-url]:  "typescript"
