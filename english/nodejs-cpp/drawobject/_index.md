---
title: DrawObject
second_title: Aspose.Cells for Node.js via C++ API Reference
description: DrawObject will be initialized and returned when rendering.
type: docs
url: /nodejs-cpp/drawobject/
---

## DrawObject class

DrawObject will be initialized and returned when rendering.

```javascript
class DrawObject;
```


## Methods

| Method | Description |
| --- | --- |
| [getCell()](#getCell--)| Indicates the Cell object when rendering. All properties of cell can be accessed. |
| [getShape()](#getShape--)| Indicates the Shape object when rendering. All properties of shape can be accessed. |
| [getImageBytes()](#getImageBytes--)| Indicates image bytes of rendered Chart, Shape when rendering. |
| [getType()](#getType--)| Indicates the type of DrawObject. |
| [getCurrentPage()](#getCurrentPage--)| Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering. |
| [getTotalPages()](#getTotalPages--)| Indicates total pages in current rendering. |
| [getSheetIndex()](#getSheetIndex--)| Indicates current sheet index of DrawObject. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getCell() {#getCell--}

Indicates the Cell object when rendering. All properties of cell can be accessed.

```javascript
getCell() : Cell;
```


**Returns**

[Cell](../cell/)

### getShape() {#getShape--}

Indicates the Shape object when rendering. All properties of shape can be accessed.

```javascript
getShape() : Shape;
```


**Returns**

[Shape](../shape/)

### getImageBytes() {#getImageBytes--}

Indicates image bytes of rendered Chart, Shape when rendering.

```javascript
getImageBytes() : number[];
```


**Returns**

number[]

### getType() {#getType--}

Indicates the type of DrawObject.

```javascript
getType() : DrawObjectEnum;
```


**Returns**

[DrawObjectEnum](../drawobjectenum/)

### getCurrentPage() {#getCurrentPage--}

Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering.

```javascript
getCurrentPage() : number;
```


### getTotalPages() {#getTotalPages--}

Indicates total pages in current rendering.

```javascript
getTotalPages() : number;
```


### getSheetIndex() {#getSheetIndex--}

Indicates current sheet index of DrawObject.

```javascript
getSheetIndex() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



