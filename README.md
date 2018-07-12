# vgg19-tensorflowjs-model

[Tensorflow.js](https://js.tensorflow.org) pretrained model of VGG-19.

## How to use it?

### Clone this repository

```sh
git clone https://github.com/DavidCai1993/vgg19-tensorflowjs-model.git
```

### Load `model.json` in your tensorflow.js application

```js
'use strict'
const tf = require('@tensorflow/tfjs')
require('@tensorflow/tfjs-node')

;(async function () {
  const vgg19 = await tf.loadModel(`file://${__dirname}/vgg19-tensorflowjs-model/model/model.json`)
  
  // ...
})(console.error)

```
