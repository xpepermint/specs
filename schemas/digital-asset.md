## Simple Summary

A convention describing **digital asset**.

## Abstract

The following convention is a [JSON Schema](http://json-schema.org/) describing a [digital asset](https://en.wikipedia.org/wiki/Digital_asset). This is the base schema from which all other schemas are extended. It follows the [ERC721 Metadata JSON Schema](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md) proposal.

## Schema

```json
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "id": "https://specs.0xcert.org/schemas/digital-asset.json",
  "description": "Represents asset metadata.",
  "properties": {
    "description": {
      "type": "string",
      "description": "Describes an asset.",
    },
    "image": {
      "type": "string",
      "description": "Points to an URI resource with mime type image/*. Consider making any images at a width between 320 and 1080 pixels and aspect ratio between 1.91:1 and 4:5 inclusive."
    },
    "name": {
      "type": "string",
      "description": "Identifies an asset.",
    }
  },
  "meta": [
    "description",
    "image",
    "name"
  ],
  "title": "DigitalAsset",
  "type": "object"
}
```
