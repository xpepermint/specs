## Simple Summary

A recipe convention describing a person.

## Abstract

The following convention is a JSON schema recipe object which describes a [Person](http://schema.org/Person) as a digital asset. The recipe provides the required and optional fields for an alive or fictional person and is meant to be used to identify and authenticate a user (e.g. KYC process).

## Schema

```json
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "description": "A person (alive or fictional).",
  "properties": {
    "additionalName": {
      "descripton": "An additional name for a Person, can be used for a middle name.",
      "type": "string"
    },
    "birthDate": {
      "description": "Date of birth.",
      "type": "string",
      "format": "date"
    },
    "birthPlace": {
      "description": "The place where the person was born.",
      "type": "string"
    },
    "email": {
      "description": "Email address.",
      "type": "string",
      "format": "email"
    },
    "familyName": {
      "description": "Family name. In the U.S., the last name of a Person.",
      "type": "string"
    },
    "gender": {
      "description": "Gender of the person.",
      "type": "string",
      "enum": ["Female", "Male"]
    },
    "givenName": {
      "description": "Given name. In the U.S., the first name of a Person.",
      "type": "string"
    }
  },
  "required": [
    "familyName",
    "gender",
    "givenName"
  ],
  "title": "Person",
  "type": "object"
}
```
