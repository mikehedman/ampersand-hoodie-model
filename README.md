# ampersand-hoodie-model

Bundles in ampersand-collection-hoodie-mixin to provide an ampersand-model that uses Hoodie for storage.

## install
```
npm install ampersand-hoodie-model
```

## example

var AmpersandHoodieModel = require('./ampersand-hoodie-model');

module.exports = AmpersandHoodieModel.extend({
    props: {
        id: 'any',
        firstName: ['string', true, ''],
        lastName: ['string', true, ''],
        coolnessFactor: ['number', true, 5]
    },
    session: {
        HOODIE_TYPE: ['string', true, 'person'],
        selected: ['boolean', true, false]
    },

## usage

The only critical usage note is that implementing classes must declare a value for the HOODIE_TYPE property.
In the example above, the HOODIE_TYPE property states that this model will be represented in Hoodie as a "person" type.

## changelog


## credits

Thanks to the Ampersand and Hoodie groups!

## license

MIT
