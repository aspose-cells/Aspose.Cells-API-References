---
title: PictureCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates a collection of Picture..picture objects.
type: docs
url: /javascript-cpp/picturecollection/
---

## PictureCollection class

Encapsulates a collection of [Picture](../picture/) objects.

```javascript
class PictureCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Picture](../picture/) element at the specified index. |
| [camera(number, number, string)](#camera-number-number-string-)| Takes a photo of the range. |
| [add(number, number, number, number, Uint8Array)](#add-number-number-number-number-uint8array-)| Adds a picture to the collection. |
| [add(number, number, number, number, string)](#add-number-number-number-number-string-)| Adds a picture to the collection. |
| [add(number, number, Uint8Array)](#add-number-number-uint8array-)| Adds a picture to the collection. |
| [add(number, number, string)](#add-number-number-string-)| Adds a picture to the collection. |
| [add(number, number, Uint8Array, number, number)](#add-number-number-uint8array-number-number-)| Adds a picture to the collection. |
| [add(number, number, string, number, number)](#add-number-number-string-number-number-)| Adds a picture to the collection. |
| [clear()](#clear--)| Clear all pictures. |
| [removeAt(number)](#removeAt-number-)| Remove shapes at the specific index |


### get(number) {#get-number-}

Gets the [Picture](../picture/) element at the specified index.

```javascript
get(index: number) : Picture;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### camera(number, number, string) {#camera-number-number-string-}

Takes a photo of the range.

```javascript
camera(row: number, column: number, range: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index of this picture. |
| column | number | The column index  of this picture. |
| range | string | The area that requires photography |

### add(number, number, number, number, Uint8Array) {#add-number-number-number-number-uint8array-}

Adds a picture to the collection.

```javascript
add(topRow: number, leftColumn: number, bottomRow: number, rightColumn: number, stream: Uint8Array) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| bottomRow | number | Lower right row index |
| rightColumn | number | Lower right column index |
| stream | Uint8Array | Stream object which contains the image data. |

**Returns**

[Picture](../picture/) object index.

### add(number, number, number, number, string) {#add-number-number-number-number-string-}

Adds a picture to the collection.

```javascript
add(topRow: number, leftColumn: number, bottomRow: number, rightColumn: number, fileName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| bottomRow | number | Lower right row index |
| rightColumn | number | Lower right column index |
| fileName | string | Image filename. |

**Returns**

[Picture](../picture/) object index.

### add(number, number, Uint8Array) {#add-number-number-uint8array-}

Adds a picture to the collection.

```javascript
add(topRow: number, leftColumn: number, stream: Uint8Array) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| stream | Uint8Array | Stream object which contains the image data. |

**Returns**

[Picture](../picture/) object index.

### add(number, number, string) {#add-number-number-string-}

Adds a picture to the collection.

```javascript
add(topRow: number, leftColumn: number, fileName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| fileName | string | Image filename. |

**Returns**

[Picture](../picture/) object index.

### add(number, number, Uint8Array, number, number) {#add-number-number-uint8array-number-number-}

Adds a picture to the collection.

```javascript
add(topRow: number, leftColumn: number, stream: Uint8Array, widthScale: number, heightScale: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| stream | Uint8Array | Stream object which contains the image data. |
| widthScale | number | Scale of image width, a percentage. |
| heightScale | number | Scale of image height, a percentage. |

**Returns**

[Picture](../picture/) object index.

### add(number, number, string, number, number) {#add-number-number-string-number-number-}

Adds a picture to the collection.

```javascript
add(topRow: number, leftColumn: number, fileName: string, widthScale: number, heightScale: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| fileName | string | Image filename. |
| widthScale | number | Scale of image width, a percentage. |
| heightScale | number | Scale of image height, a percentage. |

**Returns**

[Picture](../picture/) object index.

### clear() {#clear--}

Clear all pictures.

```javascript
clear() : void;
```


### removeAt(number) {#removeAt-number-}

Remove shapes at the specific index

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |


