---
title: Sparkline
second_title: Aspose.Cells for Node.js via C++ API Reference
description: A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.
type: docs
url: /nodejs-cpp/sparkline/
---

## Sparkline class

A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.

```javascript
class Sparkline;
```


## Methods

| Method | Description |
| --- | --- |
| [getDataRange()](#getDataRange--)| Represents the data range of the sparkline. |
| [setDataRange(string)](#setDataRange-string-)| Represents the data range of the sparkline. |
| [getRow()](#getRow--)| Gets the row index of the sparkline. |
| [getColumn()](#getColumn--)| Gets the column index of the sparkline. |
| [toImage(string, ImageOrPrintOptions)](#toImage-string-imageorprintoptions-)| Converts a sparkline to an image. |
| [toImage(ImageOrPrintOptions)](#toImage-imageorprintoptions-)| Converts a sparkline to an image. |


### getDataRange() {#getDataRange--}

Represents the data range of the sparkline.

```javascript
getDataRange() : string;
```


### setDataRange(string) {#setDataRange-string-}

Represents the data range of the sparkline.

```javascript
setDataRange(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getRow() {#getRow--}

Gets the row index of the sparkline.

```javascript
getRow() : number;
```


### getColumn() {#getColumn--}

Gets the column index of the sparkline.

```javascript
getColumn() : number;
```


### toImage(string, ImageOrPrintOptions) {#toImage-string-imageorprintoptions-}

Converts a sparkline to an image.

```javascript
toImage(fileName: string, options: ImageOrPrintOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | The image file name. |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | The image options |

### toImage(ImageOrPrintOptions) {#toImage-imageorprintoptions-}

Converts a sparkline to an image.

```javascript
toImage(options: ImageOrPrintOptions) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | The image options. |

**Returns**

The result stream


