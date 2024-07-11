---
title: PivotShowValuesSetting
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the settings about showing values as when the ShowDataAs calculation is in use.
type: docs
url: /nodejs-cpp/pivotshowvaluessetting/
---

## PivotShowValuesSetting class

Represents the settings about showing values as when the ShowDataAs calculation is in use.

```javascript
class PivotShowValuesSetting;
```


## Methods

| Method | Description |
| --- | --- |
| [getCalculationType()](#getCalculationType--)| Represents how to show values of a data field in the pivot report. |
| [setCalculationType(PivotFieldDataDisplayFormat)](#setCalculationType-pivotfielddatadisplayformat-)| Represents how to show values of a data field in the pivot report. |
| [getBaseFieldIndex()](#getBaseFieldIndex--)| Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [setBaseFieldIndex(number)](#setBaseFieldIndex-number-)| Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [getBaseItemPositionType()](#getBaseItemPositionType--)| Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [setBaseItemPositionType(PivotItemPositionType)](#setBaseItemPositionType-pivotitempositiontype-)| Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [getBaseItemIndex()](#getBaseItemIndex--)| Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. |
| [setBaseItemIndex(number)](#setBaseItemIndex-number-)| Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. |


### getCalculationType() {#getCalculationType--}

Represents how to show values of a data field in the pivot report.

```javascript
getCalculationType() : PivotFieldDataDisplayFormat;
```


**Returns**

[PivotFieldDataDisplayFormat](./pivotfielddatadisplayformat/)

### setCalculationType(PivotFieldDataDisplayFormat) {#setCalculationType-pivotfielddatadisplayformat-}

Represents how to show values of a data field in the pivot report.

```javascript
setCalculationType(value: PivotFieldDataDisplayFormat) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotFieldDataDisplayFormat](./pivotfielddatadisplayformat/) | The value to set. |

### getBaseFieldIndex() {#getBaseFieldIndex--}

Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.

```javascript
getBaseFieldIndex() : number;
```


### setBaseFieldIndex(number) {#setBaseFieldIndex-number-}

Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.

```javascript
setBaseFieldIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBaseItemPositionType() {#getBaseItemPositionType--}

Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

```javascript
getBaseItemPositionType() : PivotItemPositionType;
```


**Returns**

[PivotItemPositionType](./pivotitempositiontype/)

### setBaseItemPositionType(PivotItemPositionType) {#setBaseItemPositionType-pivotitempositiontype-}

Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

```javascript
setBaseItemPositionType(value: PivotItemPositionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotItemPositionType](./pivotitempositiontype/) | The value to set. |

### getBaseItemIndex() {#getBaseItemIndex--}

Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields.

```javascript
getBaseItemIndex() : number;
```


### setBaseItemIndex(number) {#setBaseItemIndex-number-}

Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields.

```javascript
setBaseItemIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |


