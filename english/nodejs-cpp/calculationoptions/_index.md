---
title: CalculationOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents options for calculation.
type: docs
url: /nodejs-cpp/calculationoptions/
---

## CalculationOptions class

Represents options for calculation.

```javascript
class CalculationOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getIgnoreError()](#getIgnoreError--)| Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [setIgnoreError(boolean)](#setIgnoreError-boolean-)| Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [getRecursive()](#getRecursive--)| Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |
| [setRecursive(boolean)](#setRecursive-boolean-)| Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |
| [getCustomEngine()](#getCustomEngine--)| The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [setCustomEngine(AbstractCalculationEngine)](#setCustomEngine-abstractcalculationengine-)| The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [getCalcStackSize()](#getCalcStackSize--)| The stack size for calculating cells recursively. Default value is 200. |
| [setCalcStackSize(number)](#setCalcStackSize-number-)| The stack size for calculating cells recursively. Default value is 200. |
| [getPrecisionStrategy()](#getPrecisionStrategy--)| Specifies the strategy for processing precision of calculation. |
| [setPrecisionStrategy(CalculationPrecisionStrategy)](#setPrecisionStrategy-calculationprecisionstrategy-)| Specifies the strategy for processing precision of calculation. |
| [getLinkedDataSources()](#getLinkedDataSources--)| Specifies the data sources for external links used in formulas. |
| [setLinkedDataSources(Workbook[])](#setLinkedDataSources-workbookarray-)| Specifies the data sources for external links used in formulas. |
| [getCharacterEncoding()](#getCharacterEncoding--)| Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
| [setCharacterEncoding(EncodingType)](#setCharacterEncoding-encodingtype-)| Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getIgnoreError() {#getIgnoreError--}

Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

```javascript
getIgnoreError() : boolean;
```


### setIgnoreError(boolean) {#setIgnoreError-boolean-}

Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

```javascript
setIgnoreError(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRecursive() {#getRecursive--}

Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

```javascript
getRecursive() : boolean;
```


### setRecursive(boolean) {#setRecursive-boolean-}

Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

```javascript
setRecursive(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCustomEngine() {#getCustomEngine--}

The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.

```javascript
getCustomEngine() : AbstractCalculationEngine;
```


**Returns**

[AbstractCalculationEngine](../abstractcalculationengine/)

### setCustomEngine(AbstractCalculationEngine) {#setCustomEngine-abstractcalculationengine-}

The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.

```javascript
setCustomEngine(value: AbstractCalculationEngine) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../abstractcalculationengine/) | The value to set. |

### getCalcStackSize() {#getCalcStackSize--}

The stack size for calculating cells recursively. Default value is 200.

```javascript
getCalcStackSize() : number;
```


**Remarks**

When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

### setCalcStackSize(number) {#setCalcStackSize-number-}

The stack size for calculating cells recursively. Default value is 200.

```javascript
setCalcStackSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

### getPrecisionStrategy() {#getPrecisionStrategy--}

Specifies the strategy for processing precision of calculation.

```javascript
getPrecisionStrategy() : CalculationPrecisionStrategy;
```


**Returns**

[CalculationPrecisionStrategy](../calculationprecisionstrategy/)

### setPrecisionStrategy(CalculationPrecisionStrategy) {#setPrecisionStrategy-calculationprecisionstrategy-}

Specifies the strategy for processing precision of calculation.

```javascript
setPrecisionStrategy(value: CalculationPrecisionStrategy) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CalculationPrecisionStrategy](../calculationprecisionstrategy/) | The value to set. |

### getLinkedDataSources() {#getLinkedDataSources--}

Specifies the data sources for external links used in formulas.

```javascript
getLinkedDataSources() : Workbook[];
```


**Returns**

[Workbook](../workbook/)[]

**Remarks**

Like [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/). The match of those workbooks with external links is determined by [Workbook.FileName](../workbook.filename/) and [ExternalLink.DataSource](../externallink.datasource/). So please make sure [Workbook.FileName](../workbook.filename/) has been specified with the proper value(generally it should be same with corresponding [ExternalLink.DataSource](../externallink.datasource/)) for every workbook so they can be linked as expected.

### setLinkedDataSources(Workbook[]) {#setLinkedDataSources-workbookarray-}

Specifies the data sources for external links used in formulas.

```javascript
setLinkedDataSources(value: Workbook[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Workbook](../workbook/)[] | The value to set. |

**Remarks**

Like [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/). The match of those workbooks with external links is determined by [Workbook.FileName](../workbook.filename/) and [ExternalLink.DataSource](../externallink.datasource/). So please make sure [Workbook.FileName](../workbook.filename/) has been specified with the proper value(generally it should be same with corresponding [ExternalLink.DataSource](../externallink.datasource/)) for every workbook so they can be linked as expected.

### getCharacterEncoding() {#getCharacterEncoding--}

Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

```javascript
getCharacterEncoding() : EncodingType;
```


**Returns**

[EncodingType](../encodingtype/)

### setCharacterEncoding(EncodingType) {#setCharacterEncoding-encodingtype-}

Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

```javascript
setCharacterEncoding(value: EncodingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncodingType](../encodingtype/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



