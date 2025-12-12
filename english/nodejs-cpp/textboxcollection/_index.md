---
title: TextBoxCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of TextBox..textbox objects.
type: docs
url: /nodejs-cpp/textboxcollection/
---

## TextBoxCollection class

Encapsulates a collection of [TextBox](../textbox/) objects.

```javascript
class TextBoxCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [TextBox](../textbox/) element at the specified index. |
| [get(string)](#get-string-)| Gets the [TextBox](../textbox/) element by the name. |
| [add(number, number, number, number)](#add-number-number-number-number-)| Adds a textbox to the collection. |
| [removeAt(number)](#removeAt-number-)| Remove a text box from the file. |
| [clear()](#clear--)| Clear all text boxes. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the [TextBox](../textbox/) element at the specified index.

```javascript
get(index: number) : TextBox;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### get(string) {#get-string-}

Gets the [TextBox](../textbox/) element by the name.

```javascript
get(name: string) : TextBox;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the text box. |

**Returns**

[TextBox](../textbox/)

### add(number, number, number, number) {#add-number-number-number-number-}

Adds a textbox to the collection.

```javascript
add(topRow: number, leftColumn: number, height: number, width: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| height | number | Height of textbox, in unit of pixel. |
| width | number | Width of textbox, in unit of pixel. |

**Returns**

[TextBox](../textbox/) object index.

### removeAt(number) {#removeAt-number-}

Remove a text box from the file.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The text box index. |

### clear() {#clear--}

Clear all text boxes.

```javascript
clear() : void;
```


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



