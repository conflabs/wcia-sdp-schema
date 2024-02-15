# WCIA SDP Schema
A schema description of the Strain Data Project (SDP) object sometimes included in WCIA lab transfer schema's meta field.

# Current Version 1.0.0

----

- [About the Strain Data Project](https://straindataproject.org/)
- [WCIA Lab Result Schema](https://www.github.com/conflabs/wcia-lab-result-schema)
- [WCIA Transfer Data Schema](https://github.com/conflabs/wcia-transfer-data-schema)

----

# Strain Data Project Object

[The Strain Data Project (SDP)](https://straindataproject.org/) object is a JSON object that is included in the 
[WCIA Lab Transfer Schema](https://www.github.com/conflabs/wcia-lab-result-schema) by participating laboratories. The SDP 
object is optional and may be omitted from the lab transfer schema. It is used to provide SDP information and assets 
related to the sample being tested.

## Legend

```txt
Ln #    Schema                     Description
----    -----------------------    ---------------------------------------------------------------------------------
  1     meta                       The meta object of the lab transfer schema.
  2     └── sdp                    An object containing property/value pairs related to the Strain Data Project.
  3         ├── sdp_category       A string value representing the category of the sample.
  4         ├── sdp_color          A string value representing the category of the sample.
  5         ├── sdp_thumbnail      A string value representing the URL of a thumbnail image asset for the sample.
  6         └── sdp_compass        A string value representing the URL of a compass image asset for the sample.

### Example: ###
 
"meta": {
    "sdp": {
        "sdp_category": "string",
        "sdp_color": "string",
        "sdp_thumbnail": "string",
        "sdp_compass": "string"
    }
}
```

## Fields Guide

----

### The Lab Result Transfer Meta Object

- _Field Name:_ **meta**
- _Type:_ Object
- _Description:_ The meta object of the lab transfer schema.
- _Legend_: Ln #1

### The Strain Data Project Object

- _Field Name:_ **sdp**
- _Type:_ Object
- _Description:_ An object containing property/value pairs related to the Strain Data Project.
- _Legend_: Ln #2

### The Strain Data Project Category

- _Field Name:_ **sdp_category**
- _Type:_ String
- _Description:_ A string value representing the category of the sample. It is a single letter.
- _Legend_: Ln #3

### The Strain Data Project Color

- _Field Name:_ **sdp_color**
- _Type:_ String
- _Description:_ A string value representing the color of the sample. It is a complete word.
- _Legend_: Ln #4

### The Strain Data Project Thumbnail

- _Field Name:_ **sdp_thumbnail**
- _Type:_ String
- _Description:_ A string value representing the URL of a thumbnail image asset for the sample. Usually a png.
- _Legend_: Ln #5

### The Strain Data Project Compass

- _Field Name:_ **sdp_compass**
- _Type:_ String
- _Description:_ A string value representing the URL of a compass image asset for the sample. Usually a png.
- _Legend_: Ln #6

