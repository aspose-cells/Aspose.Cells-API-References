---
title: CheckBoxCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection of CheckBoxnodejscppcheckbox objects in a worksheet.
type: docs
url: /nodejs-cpp/checkboxcollection/
---

## CheckBoxCollection class

Represents a collection of [CheckBox](/nodejs-cpp/checkbox/) objects in a worksheet.

```javascript
class CheckBoxCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [CheckBox](/nodejs-cpp/checkbox/) element at the specified index. |
| [add(number, number, number, number)](#add-number-number-number-number-)| Adds a checkBox to the collection. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets the [CheckBox](/nodejs-cpp/checkbox/) element at the specified index.

```javascript
get(index: number) : CheckBox;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### add(number, number, number, number) {#add-number-number-number-number-}

Adds a checkBox to the collection.

```javascript
add(upperLeftRow: number, upperLeftColumn: number, height: number, width: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| height | number | Height of checkBox, in unit of pixel. |
| width | number | Width of checkBox, in unit of pixel. |

**Returns**

[CheckBox](/nodejs-cpp/checkbox/) object index.

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



