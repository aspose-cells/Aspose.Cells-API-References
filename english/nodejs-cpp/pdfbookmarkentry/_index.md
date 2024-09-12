---
title: PdfBookmarkEntry
second_title: Aspose.Cells for Node.js via C++ API Reference
description: PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or  current instance will be hidden and children will be inserted on current level.
type: docs
url: /nodejs-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or "", current instance will be hidden and children will be inserted on current level.

```javascript
class PdfBookmarkEntry;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getText()](#getText--)| Title of a bookmark. |
| [setText(string)](#setText-string-)| Title of a bookmark. |
| [getDestination()](#getDestination--)| The cell to which the bookmark link. |
| [setDestination(Cell)](#setDestination-cell-)| The cell to which the bookmark link. |
| [getDestinationName()](#getDestinationName--)| Gets or sets name of destination. |
| [setDestinationName(string)](#setDestinationName-string-)| Gets or sets name of destination. |
| [isOpen()](#isOpen--)| When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [setIsOpen(boolean)](#setIsOpen-boolean-)| When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [isCollapse()](#isCollapse--)| When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
| [setIsCollapse(boolean)](#setIsCollapse-boolean-)| When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getText() {#getText--}

Title of a bookmark.

```javascript
getText() : string;
```


### setText(string) {#setText-string-}

Title of a bookmark.

```javascript
setText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDestination() {#getDestination--}

The cell to which the bookmark link.

```javascript
getDestination() : Cell;
```


**Returns**

[Cell](../cell/)

### setDestination(Cell) {#setDestination-cell-}

The cell to which the bookmark link.

```javascript
setDestination(value: Cell) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Cell](../cell/) | The value to set. |

### getDestinationName() {#getDestinationName--}

Gets or sets name of destination.

```javascript
getDestinationName() : string;
```


**Remarks**

If destination name is set, the destination will be defined as a named destination with this name.

### setDestinationName(string) {#setDestinationName-string-}

Gets or sets name of destination.

```javascript
setDestinationName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If destination name is set, the destination will be defined as a named destination with this name.

### isOpen() {#isOpen--}

When this property is true, the bookmarkentry will expand, otherwise it will collapse.

```javascript
isOpen() : boolean;
```


### setIsOpen(boolean) {#setIsOpen-boolean-}

When this property is true, the bookmarkentry will expand, otherwise it will collapse.

```javascript
setIsOpen(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isCollapse() {#isCollapse--}

When this property is true, the bookmarkentry will collapse, otherwise it will expand.

```javascript
isCollapse() : boolean;
```


### setIsCollapse(boolean) {#setIsCollapse-boolean-}

When this property is true, the bookmarkentry will collapse, otherwise it will expand.

```javascript
setIsCollapse(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



