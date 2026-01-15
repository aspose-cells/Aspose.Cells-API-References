---
title: GradientStopCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the gradient stop collection.
type: docs
url: /nodejs-cpp/gradientstopcollection/
---

## GradientStopCollection class

Represents the gradient stop collection.

```javascript
class GradientStopCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the gradient stop by the index. |
| [add(number, CellsColor, number)](#add-number-cellscolor-number-)| Add a gradient stop. |
| [add(number, Color, number)](#add-number-color-number-)| Add a gradient stop. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the gradient stop by the index.

```javascript
get(index: number) : GradientStop;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

The gradient stop.

### add(number, CellsColor, number) {#add-number-cellscolor-number-}

Add a gradient stop.

```javascript
add(position: number, color: CellsColor, alpha: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| position | number | The position of the stop,in unit of percentage. |
| color | [CellsColor](../cellscolor/) | The color of the stop. |
| alpha | number | The alpha of the color. |

### add(number, Color, number) {#add-number-color-number-}

Add a gradient stop.

```javascript
add(position: number, color: Color, alpha: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| position | number | The position of the stop,in unit of percentage. |
| color | [Color](../color/) | The color of the stop. |
| alpha | number | The alpha of the color. |

### getCount() {#getCount--}

<b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



