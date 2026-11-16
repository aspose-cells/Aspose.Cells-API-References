---
title: PivotShowValuesSetting
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the settings about showing values as when the ShowDataAs calculation is in use.
type: docs
url: /javascript-cpp/pivotshowvaluessetting/
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


