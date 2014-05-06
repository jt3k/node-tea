*Block TEA (xxtea) Tiny Encryption Algorithm implementation in JavaScript as a Node module*

A complete copy paste of code from http://www.movable-type.co.uk/scripts/tea-block.html

## Install

To install packnode, use [npm](http://github.com/isaacs/npm)

    $ npm install tea

## Usage

```javascript
var tea = require('tea');

var clear     = 'string to be encrypted';
var password  = 'BH&^!   ljknca>":{L{}uuj~``BF';
var encrypted = tea.encrypt(clear,     password);
var decrypted = tea.decrypt(encrypted, password);

console.log(clear, encrypted, decrypted);
//--> 'string to be encrypted', 'xR4q8OXWSShGk/LYrCQNLWET1GtXooG3', 'string to be encrypted'
```