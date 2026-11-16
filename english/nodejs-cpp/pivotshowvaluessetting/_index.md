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


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [showValuesAs](#showValuesAs--)| PivotShowValuesAsType | Gets and sets how to show values of a data field in the pivot report. |
| [calculationType](#calculationType--)| PivotFieldDataDisplayFormat | Represents how to show values of a data field in the pivot report. |
| [baseFieldIndex](#baseFieldIndex--)| number | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [baseItemPositionType](#baseItemPositionType--)| PivotItemPositionType | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [baseFieldName](#baseFieldName--)| string | Readonly. Gets caption of the pivot base field. |
| [baseItemCaption](#baseItemCaption--)| string | Readonly. Gets caption of the pivot item in the base field. |
| [baseItemIndex](#baseItemIndex--)| number | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. |

## Methods

| Method | Description |
| --- | --- |
| [getShowValuesAs()](#getShowValuesAs--)| <b>@deprecated.</b> Please use the 'showValuesAs' property instead. Gets and sets how to show values of a data field in the pivot report. |
| [setShowValuesAs(PivotShowValuesAsType)](#setShowValuesAs-pivotshowvaluesastype-)| <b>@deprecated.</b> Please use the 'showValuesAs' property instead. Gets and sets how to show values of a data field in the pivot report. |
| [getCalculationType()](#getCalculationType--)| <b>@deprecated.</b> Please use the 'calculationType' property instead. Represents how to show values of a data field in the pivot report. |
| [setCalculationType(PivotFieldDataDisplayFormat)](#setCalculationType-pivotfielddatadisplayformat-)| <b>@deprecated.</b> Please use the 'calculationType' property instead. Represents how to show values of a data field in the pivot report. |
| [getBaseFieldIndex()](#getBaseFieldIndex--)| <b>@deprecated.</b> Please use the 'baseFieldIndex' property instead. Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [setBaseFieldIndex(number)](#setBaseFieldIndex-number-)| <b>@deprecated.</b> Please use the 'baseFieldIndex' property instead. Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [getBaseItemPositionType()](#getBaseItemPositionType--)| <b>@deprecated.</b> Please use the 'baseItemPositionType' property instead. Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [setBaseItemPositionType(PivotItemPositionType)](#setBaseItemPositionType-pivotitempositiontype-)| <b>@deprecated.</b> Please use the 'baseItemPositionType' property instead. Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [getBaseFieldName()](#getBaseFieldName--)| <b>@deprecated.</b> Please use the 'baseFieldName' property instead. Gets caption of the pivot base field. |
| [getBaseItemCaption()](#getBaseItemCaption--)| <b>@deprecated.</b> Please use the 'baseItemCaption' property instead. Gets caption of the pivot item in the base field. |
| [getBaseItemIndex()](#getBaseItemIndex--)| <b>@deprecated.</b> Please use the 'baseItemIndex' property instead. Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. |
| [setBaseItemIndex(number)](#setBaseItemIndex-number-)| <b>@deprecated.</b> Please use the 'baseItemIndex' property instead. Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### showValuesAs {#showValuesAs--}

Gets and sets how to show values of a data field in the pivot report.

```javascript
showValuesAs : PivotShowValuesAsType;
```


### calculationType {#calculationType--}

Represents how to show values of a data field in the pivot report.

```javascript
calculationType : PivotFieldDataDisplayFormat;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.ShowValuesAs property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

### baseFieldIndex {#baseFieldIndex--}

Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.

```javascript
baseFieldIndex : number;
```


### baseItemPositionType {#baseItemPositionType--}

Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

```javascript
baseItemPositionType : PivotItemPositionType;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.BaseItem property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

### baseFieldName {#baseFieldName--}

Readonly. Gets caption of the pivot base field.

```javascript
baseFieldName : string;
```


### baseItemCaption {#baseItemCaption--}

Readonly. Gets caption of the pivot item in the base field.

```javascript
baseItemCaption : string;
```


### baseItemIndex {#baseItemIndex--}

Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use.

```javascript
baseItemIndex : number;
```


**Remarks**

[PivotShowValuesSetting.PreviousPivotItem](../pivotshowvaluessetting.previouspivotitem/) (-1) for the preceding item, [PivotShowValuesSetting.NextPivotItem](../pivotshowvaluessetting.nextpivotitem/) (-2) for the succeeding item; non‑negative values denote the ordinal index of a specific pivot item.

### getShowValuesAs() {#getShowValuesAs--}

<b>@deprecated.</b> Please use the 'showValuesAs' property instead. Gets and sets how to show values of a data field in the pivot report.

```javascript
getShowValuesAs() : PivotShowValuesAsType;
```


**Returns**

[PivotShowValuesAsType](../pivotshowvaluesastype/)

### setShowValuesAs(PivotShowValuesAsType) {#setShowValuesAs-pivotshowvaluesastype-}

<b>@deprecated.</b> Please use the 'showValuesAs' property instead. Gets and sets how to show values of a data field in the pivot report.

```javascript
setShowValuesAs(value: PivotShowValuesAsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotShowValuesAsType](../pivotshowvaluesastype/) | The value to set. |

### getCalculationType() {#getCalculationType--}

<b>@deprecated.</b> Please use the 'calculationType' property instead. Represents how to show values of a data field in the pivot report.

```javascript
getCalculationType() : PivotFieldDataDisplayFormat;
```


**Returns**

[PivotFieldDataDisplayFormat](../pivotfielddatadisplayformat/)

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.ShowValuesAs property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

### setCalculationType(PivotFieldDataDisplayFormat) {#setCalculationType-pivotfielddatadisplayformat-}

<b>@deprecated.</b> Please use the 'calculationType' property instead. Represents how to show values of a data field in the pivot report.

```javascript
setCalculationType(value: PivotFieldDataDisplayFormat) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotFieldDataDisplayFormat](../pivotfielddatadisplayformat/) | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.ShowValuesAs property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

### getBaseFieldIndex() {#getBaseFieldIndex--}

<b>@deprecated.</b> Please use the 'baseFieldIndex' property instead. Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.

```javascript
getBaseFieldIndex() : number;
```


### setBaseFieldIndex(number) {#setBaseFieldIndex-number-}

<b>@deprecated.</b> Please use the 'baseFieldIndex' property instead. Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.

```javascript
setBaseFieldIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBaseItemPositionType() {#getBaseItemPositionType--}

<b>@deprecated.</b> Please use the 'baseItemPositionType' property instead. Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

```javascript
getBaseItemPositionType() : PivotItemPositionType;
```


**Returns**

[PivotItemPositionType](../pivotitempositiontype/)

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.BaseItem property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

### setBaseItemPositionType(PivotItemPositionType) {#setBaseItemPositionType-pivotitempositiontype-}

<b>@deprecated.</b> Please use the 'baseItemPositionType' property instead. Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

```javascript
setBaseItemPositionType(value: PivotItemPositionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotItemPositionType](../pivotitempositiontype/) | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.BaseItem property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

### getBaseFieldName() {#getBaseFieldName--}

<b>@deprecated.</b> Please use the 'baseFieldName' property instead. Gets caption of the pivot base field.

```javascript
getBaseFieldName() : string;
```


### getBaseItemCaption() {#getBaseItemCaption--}

<b>@deprecated.</b> Please use the 'baseItemCaption' property instead. Gets caption of the pivot item in the base field.

```javascript
getBaseItemCaption() : string;
```


### getBaseItemIndex() {#getBaseItemIndex--}

<b>@deprecated.</b> Please use the 'baseItemIndex' property instead. Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use.

```javascript
getBaseItemIndex() : number;
```


**Remarks**

[PivotShowValuesSetting.PreviousPivotItem](../pivotshowvaluessetting.previouspivotitem/) (-1) for the preceding item, [PivotShowValuesSetting.NextPivotItem](../pivotshowvaluessetting.nextpivotitem/) (-2) for the succeeding item; non‑negative values denote the ordinal index of a specific pivot item.

### setBaseItemIndex(number) {#setBaseItemIndex-number-}

<b>@deprecated.</b> Please use the 'baseItemIndex' property instead. Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use.

```javascript
setBaseItemIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

[PivotShowValuesSetting.PreviousPivotItem](../pivotshowvaluessetting.previouspivotitem/) (-1) for the preceding item, [PivotShowValuesSetting.NextPivotItem](../pivotshowvaluessetting.nextpivotitem/) (-2) for the succeeding item; non‑negative values denote the ordinal index of a specific pivot item.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



