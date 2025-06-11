﻿---
title: CustomRenderSettings
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents custom settings during rendering.
type: docs
url: /nodejs-cpp/customrendersettings/
---

## CustomRenderSettings class

Represents custom settings during rendering.

```javascript
class CustomRenderSettings;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Ctor. |

## Methods

| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getCellBorderWidth(CellBorderType)](#getCellBorderWidth-cellbordertype-)| Get cell border width according to border type. |


### constructor() {#constructor--}

Ctor.

```javascript
constructor();
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getCellBorderWidth(CellBorderType) {#getCellBorderWidth-cellbordertype-}

Get cell border width according to border type.

```javascript
getCellBorderWidth(borderType: CellBorderType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | [CellBorderType](../cellbordertype/) | cell border type |

**Returns**

cell border width

**Remarks**

Any negative value will be ignored.


