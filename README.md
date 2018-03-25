# [0xcert](https://0xcert.org)/specs

> Conventions, recipes and other specs for 0xcert protocol.

## Recipes

A digital asset in the 0xcert protocol is defined and described in form of a specifically designed JSON object, which conforms to [RFC-7159](https://en.wikipedia.org/wiki/JSON) and follows the mapping format defined by the [JSON schema](http://json-schema.org) specification.

The protocol provides conventions for these objects, thus every digital asset in the 0xcert protocol has its own Xcert recipe. The Xcert recipe represents a technical specification of a particular digital asset, which explains the JSON object structure and a detailed description of each data key.

The naming of JSON properties must follow the [schema.org](http://schema.org/) specification when possible. This is to enable an easy way to convert a digital asset data object into JSON-LD format. The convention expects the JSON keys to be defined in alphabetical order.

Anyone can propose a new Xcert recipe by opening a new [issue](/issues). The document is accepted and merged into master branch when the interested community approves it based on the majority consensus.

## License

```
Copyright (c) 2017+ 0xcert <admin@0xcert.org>
```
