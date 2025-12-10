---
title: OleObjectCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents embedded OLE objects.
type: docs
url: /nodejs-cpp/oleobjectcollection/
---

## OleObjectCollection class

Represents embedded OLE objects.

```javascript
class OleObjectCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [OleObject](../oleobject/) element at the specified index. |
| [add(number, number, number, number, Uint8Array)](#add-number-number-number-number-uint8array-)| Adds an OleObject to the collection. |
| [add(number, number, number, number, Uint8Array, string)](#add-number-number-number-number-uint8array-string-)| Adds a linked OleObject to the collection. |
| [clear()](#clear--)| Remove all embedded OLE objects. |
| [removeAt(number)](#removeAt-number-)| Removes the element at the specified index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the [OleObject](../oleobject/) element at the specified index.

```javascript
get(index: number) : OleObject;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### add(number, number, number, number, Uint8Array) {#add-number-number-number-number-uint8array-}

Adds an OleObject to the collection.

```javascript
add(topRow: number, leftColumn: number, height: number, width: number, imageData: Uint8Array) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| height | number | Height of oleObject, in unit of pixel. |
| width | number | Width of oleObject, in unit of pixel. |
| imageData | number[] | Image of ole object as byte array. |

**Returns**

[OleObject](../oleobject/) object index.

### add(number, number, number, number, Uint8Array, string) {#add-number-number-number-number-uint8array-string-}

Adds a linked OleObject to the collection.

```javascript
add(topRow: number, leftColumn: number, height: number, width: number, imageData: Uint8Array, linkedFile: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| height | number | Height of oleObject, in unit of pixel. |
| width | number | Width of oleObject, in unit of pixel. |
| imageData | number[] | Image of ole object as byte array. |
| linkedFile | string |  |

**Returns**

[OleObject](../oleobject/) object index.

### clear() {#clear--}

Remove all embedded OLE objects.

```javascript
clear() : void;
```


### removeAt(number) {#removeAt-number-}

Removes the element at the specified index.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The specified index. |

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



