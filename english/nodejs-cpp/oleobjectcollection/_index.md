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
| [add(number, number, number, number, number[])](#add-number-number-number-number-numberarray-)| Adds an OleObject to the collection. |
| [add(number, number, number, number, number[], string)](#add-number-number-number-number-numberarray-string-)| Adds a linked OleObject to the collection. |
| [clear()](#clear--)| Remove all embedded OLE objects. |
| [removeAt(number)](#removeAt-number-)| Removes the element at the specified index. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


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

### add(number, number, number, number, number[]) {#add-number-number-number-number-numberarray-}

Adds an OleObject to the collection.

```javascript
add(upperLeftRow: number, upperLeftColumn: number, height: number, width: number, imageData: number[]) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| height | number | Height of oleObject, in unit of pixel. |
| width | number | Width of oleObject, in unit of pixel. |
| imageData | number[] | Image of ole object as byte array. |

**Returns**

[OleObject](../oleobject/) object index.

### add(number, number, number, number, number[], string) {#add-number-number-number-number-numberarray-string-}

Adds a linked OleObject to the collection.

```javascript
add(upperLeftRow: number, upperLeftColumn: number, height: number, width: number, imageData: number[], linkedFile: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
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

Gets the number of elements contained in.

```javascript
getCount() : number;
```



