---
title: AutoFitterOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all auto fitter options.
type: docs
url: /nodejs-cpp/autofitteroptions/
---

## AutoFitterOptions class

Represents all auto fitter options.

```javascript
class AutoFitterOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--)| Gets or sets default edit language. |
| [setDefaultEditLanguage(DefaultEditLanguage)](#setDefaultEditLanguage-defaulteditlanguage-)| Gets or sets default edit language. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--)| Gets and set the type of auto fitting row height of merged cells. |
| [setAutoFitMergedCellsType(AutoFitMergedCellsType)](#setAutoFitMergedCellsType-autofitmergedcellstype-)| Gets and set the type of auto fitting row height of merged cells. |
| [getOnlyAuto()](#getOnlyAuto--)| Indicates whether only fit the rows which height are not customed. |
| [setOnlyAuto(boolean)](#setOnlyAuto-boolean-)| Indicates whether only fit the rows which height are not customed. |
| [getIgnoreHidden()](#getIgnoreHidden--)| Ignores the hidden rows/columns. |
| [setIgnoreHidden(boolean)](#setIgnoreHidden-boolean-)| Ignores the hidden rows/columns. |
| [getMaxRowHeight()](#getMaxRowHeight--)| Gets and sets the max row height(in unit of Point) when autofitting rows. |
| [setMaxRowHeight(number)](#setMaxRowHeight-number-)| Gets and sets the max row height(in unit of Point) when autofitting rows. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--)| Gets and sets the type of auto fitting wrapped text. |
| [setAutoFitWrappedTextType(AutoFitWrappedTextType)](#setAutoFitWrappedTextType-autofitwrappedtexttype-)| Gets and sets the type of auto fitting wrapped text. |
| [getFormatStrategy()](#getFormatStrategy--)| Gets and sets the formatted strategy. |
| [setFormatStrategy(CellValueFormatStrategy)](#setFormatStrategy-cellvalueformatstrategy-)| Gets and sets the formatted strategy. |
| [getForRendering()](#getForRendering--)| Indicates whether fit for rendering purpose. |
| [setForRendering(boolean)](#setForRendering-boolean-)| Indicates whether fit for rendering purpose. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getDefaultEditLanguage() {#getDefaultEditLanguage--}

Gets or sets default edit language.

```javascript
getDefaultEditLanguage() : DefaultEditLanguage;
```


**Returns**

[DefaultEditLanguage](/nodejs-cpp/defaulteditlanguage/)

**Remarks**

It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](/nodejs-cpp/aspose.cells.defaulteditlanguage.auto/).

### setDefaultEditLanguage(DefaultEditLanguage) {#setDefaultEditLanguage-defaulteditlanguage-}

Gets or sets default edit language.

```javascript
setDefaultEditLanguage(value: DefaultEditLanguage) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DefaultEditLanguage](/nodejs-cpp/defaulteditlanguage/) | The value to set. |

**Remarks**

It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](/nodejs-cpp/aspose.cells.defaulteditlanguage.auto/).

### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}

Gets and set the type of auto fitting row height of merged cells.

```javascript
getAutoFitMergedCellsType() : AutoFitMergedCellsType;
```


**Returns**

[AutoFitMergedCellsType](/nodejs-cpp/autofitmergedcellstype/)

**Remarks**

Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.

### setAutoFitMergedCellsType(AutoFitMergedCellsType) {#setAutoFitMergedCellsType-autofitmergedcellstype-}

Gets and set the type of auto fitting row height of merged cells.

```javascript
setAutoFitMergedCellsType(value: AutoFitMergedCellsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoFitMergedCellsType](/nodejs-cpp/autofitmergedcellstype/) | The value to set. |

**Remarks**

Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.

### getOnlyAuto() {#getOnlyAuto--}

Indicates whether only fit the rows which height are not customed.

```javascript
getOnlyAuto() : boolean;
```


### setOnlyAuto(boolean) {#setOnlyAuto-boolean-}

Indicates whether only fit the rows which height are not customed.

```javascript
setOnlyAuto(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIgnoreHidden() {#getIgnoreHidden--}

Ignores the hidden rows/columns.

```javascript
getIgnoreHidden() : boolean;
```


### setIgnoreHidden(boolean) {#setIgnoreHidden-boolean-}

Ignores the hidden rows/columns.

```javascript
setIgnoreHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMaxRowHeight() {#getMaxRowHeight--}

Gets and sets the max row height(in unit of Point) when autofitting rows.

```javascript
getMaxRowHeight() : number;
```


### setMaxRowHeight(number) {#setMaxRowHeight-number-}

Gets and sets the max row height(in unit of Point) when autofitting rows.

```javascript
setMaxRowHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}

Gets and sets the type of auto fitting wrapped text.

```javascript
getAutoFitWrappedTextType() : AutoFitWrappedTextType;
```


**Returns**

[AutoFitWrappedTextType](/nodejs-cpp/autofitwrappedtexttype/)

### setAutoFitWrappedTextType(AutoFitWrappedTextType) {#setAutoFitWrappedTextType-autofitwrappedtexttype-}

Gets and sets the type of auto fitting wrapped text.

```javascript
setAutoFitWrappedTextType(value: AutoFitWrappedTextType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoFitWrappedTextType](/nodejs-cpp/autofitwrappedtexttype/) | The value to set. |

### getFormatStrategy() {#getFormatStrategy--}

Gets and sets the formatted strategy.

```javascript
getFormatStrategy() : CellValueFormatStrategy;
```


**Returns**

[CellValueFormatStrategy](/nodejs-cpp/cellvalueformatstrategy/)

**Remarks**

The default value is CellStyle for performance.

### setFormatStrategy(CellValueFormatStrategy) {#setFormatStrategy-cellvalueformatstrategy-}

Gets and sets the formatted strategy.

```javascript
setFormatStrategy(value: CellValueFormatStrategy) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellValueFormatStrategy](/nodejs-cpp/cellvalueformatstrategy/) | The value to set. |

**Remarks**

The default value is CellStyle for performance.

### getForRendering() {#getForRendering--}

Indicates whether fit for rendering purpose.

```javascript
getForRendering() : boolean;
```


### setForRendering(boolean) {#setForRendering-boolean-}

Indicates whether fit for rendering purpose.

```javascript
setForRendering(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |


