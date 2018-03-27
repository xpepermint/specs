## Simple Summary

A convention describing a **message digest** digital asset.

## Abstract

The following convention is a [JSON Schema](http://json-schema.org) describing a [message digest](https://en.wikipedia.org/wiki/Cryptographic_hash_function) digital asset. A message digest represents the returned value of a cryptographic hash function. The function generates a hash using a mathematical algorithm. The hash can then be used to uniquely identify secret information.

## Schema

```json
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "allOf": [
    {
      "$ref": "digital-asset.json"
    },
    {
      "meta": [
        "digestAlgorithm",
        "digestValue"
      ],
      "proof": [
        "digestAlgorithm",
        "digestValue"
      ],
      "properties": {
        "digestAlgorithm": {
          "description": "Represents a cryptographic algorithm.",
          "enum": ["sha256", "sha512"],
          "type": "string"
        },
        "digestValue": {
          "description": "Represents a cryptographic hash.",
          "type": "string"
        }
      },
      "required": [
        "digestAlgorithm",
        "digestValue"
      ],
    }
  ],
  "description": "A message digest of a cryptographic hash function.",
  "id": "https://specs.0xcert.org/schemas/message-digest.json",
  "title": "MessageDigest",
  "type": "object"
}
```
