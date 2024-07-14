---
title: TextTabStopCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the list of all tab stops.
type: docs
url: /nodejs-cpp/texttabstopcollection/
---

## TextTabStopCollection class

Represents the list of all tab stops.

```javascript
class TextTabStopCollection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [TextTabStop](/nodejs-cpp/texttabstop/) by the index. |
| [add(TextTabAlignmentType, number)](#add-texttabalignmenttype-number-)| Adds a tab stop. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### get(number) {#get-number-}

Gets [TextTabStop](/nodejs-cpp/texttabstop/) by the index.

```javascript
get(index: number) : TextTabStop;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[TextTabStop](/nodejs-cpp/texttabstop/)

### add(TextTabAlignmentType, number) {#add-texttabalignmenttype-number-}

Adds a tab stop.

```javascript
add(tabAlignment: TextTabAlignmentType, tabPosition: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tabAlignment | [TextTabAlignmentType](/nodejs-cpp/texttabalignmenttype/) |  |
| tabPosition | number |  |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



