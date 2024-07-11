---
title: Color
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents an ARGB (alpha, red, green, blue) color.
type: docs
url: /nodejs-cpp/color/
---

## Color class
Represents an ARGB (alpha, red, green, blue) color.


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
| [constructor(number, number, number)](#constructor-number-number-number-)| Constructs a Color object from the specified 8-bit color values (red, green, and blue). |
| [constructor(number, number, number, number)](#constructor-number-number-number-number-)| Constructs a Color object from the four ARGB component (alpha, red, green, and blue) values. |

## Properties

| Name | Description |
| --- | --- |
| a | Gets or sets the alpha component value of this Color class. |
| r | Gets or sets the red component value of this Color class. |
| g | Gets or sets the green component value of this Color class. |
| b | Gets or sets the blue component value of this Color class. |

## Methods

| Method | Description |
| --- | --- |
| [equals(Color)](#equals-color-)| Determines whether the specified color is equal to the current color. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```

### constructor(number, number, number) {#constructor-number-number-number-}

Constructs a Color object from the specified 8-bit color values (red, green, and blue).

```javascript
constructor(r: number, g: number, b: number);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| r | number | The red component value(0~255). |
| g | number | The green component value(0~255). |
| b | number | The blue component value(0~255). |

### constructor(number, number, number, number) {#constructor-number-number-number-number-}

Constructs a Color object from the four ARGB component (alpha, red, green, and blue) values.

```javascript
constructor(a: number, r: number, g: number, b: number);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | number | The alpha component value(0~255). |
| r | number | The red component value(0~255). |
| g | number | The green component value(0~255). |
| b | number | The blue component value(0~255). |

### equals(Color) {##equals-color-}

Determines whether the specified color is equal to the current color.

```javascript
equals(color: Color): boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | An color to compare with this color. |

**Returns**

true if the current color is equal to other; otherwise, false.
