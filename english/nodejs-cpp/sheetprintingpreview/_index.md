﻿---
title: SheetPrintingPreview
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Worksheet printing preview.
type: docs
url: /nodejs-cpp/sheetprintingpreview/
---

## SheetPrintingPreview class

Worksheet printing preview.

```javascript
class SheetPrintingPreview;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor(Worksheet, ImageOrPrintOptions)](#constructor-worksheet-imageorprintoptions-)| The construct of SheetPrintingPreview |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [evaluatedPageCount](#evaluatedPageCount--)| number | Readonly. Evaluate the total page count of this worksheet |

## Methods

| Method | Description |
| --- | --- |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--)| <b>@deprecated.</b> Please use the 'evaluatedPageCount' property instead. Evaluate the total page count of this worksheet |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor(Worksheet, ImageOrPrintOptions) {#constructor-worksheet-imageorprintoptions-}

The construct of SheetPrintingPreview

```javascript
constructor(sheet: Worksheet, options: ImageOrPrintOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../worksheet/) | Indicate which spreadsheet to be printed. |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | ImageOrPrintOptions contains some property of output |

### evaluatedPageCount {#evaluatedPageCount--}

Readonly. Evaluate the total page count of this worksheet

```javascript
evaluatedPageCount : number;
```


### getEvaluatedPageCount() {#getEvaluatedPageCount--}

<b>@deprecated.</b> Please use the 'evaluatedPageCount' property instead. Evaluate the total page count of this worksheet

```javascript
getEvaluatedPageCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



