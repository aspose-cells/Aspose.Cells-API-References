---
title: Aspose::Cells::Pivot::PivotField::ShowValuesAs method
linktitle: ShowValuesAs
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotField::ShowValuesAs method. Shows values of data field as different display format when the ShowDataAs calculation is in use in C++.'
type: docs
weight: 8900
url: /cpp/aspose.cells.pivot/pivotfield/showvaluesas/
---
## PivotField::ShowValuesAs(PivotFieldDataDisplayFormat, int32_t, PivotItemPositionType, int32_t) method


Shows values of data field as different display format when the ShowDataAs calculation is in use.


>Deprecated
>
>Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead. 
```cpp
void Aspose::Cells::Pivot::PivotField::ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int32_t baseField, PivotItemPositionType baseItemPositionType, int32_t baseItem)
```


| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | The data display format type. |
| baseField | int32_t | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | PivotItemPositionType | The position type of base iteam. |
| baseItem | int32_t | The index to the base item which ShowDataAs calculation bases on. Only works when baseItemPositionType is custom. |
## Remarks



NOTE: This property is now obsolete. Instead, please use [PivotField.ShowValuesAs(PivotShowValuesAsType,int,int)](./) method instead. This method will be removed 12 months later since November 2026. **Aspose** apologizes for any inconvenience you may have experienced. 


## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* Enum [PivotItemPositionType](../../pivotitempositiontype/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::ShowValuesAs(PivotShowValuesAsType, int32_t, int32_t) method


Sets the "Show Values As" calculation for this pivot field.

```cpp
void Aspose::Cells::Pivot::PivotField::ShowValuesAs(PivotShowValuesAsType showValuesAsType, int32_t baseField, int32_t baseItem)
```


| Parameter | Type | Description |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Type of the "Show Values As" calculation. |
| baseField | int32_t | Index of the base field used for the calculation. |
| baseItem | int32_t | Index of the base item for the calculation. Use PivotShowValuesSetting.PreviousPivotItem (-1) for the preceding item, PivotShowValuesSetting.NextPivotItem (-2) for the succeeding item; non‑negative values denote the ordinal index of a specific pivot item. |
## Remarks



Only for data field. 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::ShowValuesAs(PivotShowValuesAsType, const U16String\&, const U16String\&) method


Configures the "Show Values As" calculation for this data field.

```cpp
void Aspose::Cells::Pivot::PivotField::ShowValuesAs(PivotShowValuesAsType showValuesAsType, const U16String &baseField, const U16String &baseItem)
```


| Parameter | Type | Description |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | The calculation type for Show Values As. |
| baseField | const U16String\& | The name of the base field used in the calculation. |
| baseItem | const U16String\& | Caption of a regular pivot item. Also accepts reserved literal keywords: **(previous)** for the previous item, **(next)** for the next item. Pass **null** if the selected calculation type does not require a base item. |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::ShowValuesAs(PivotShowValuesAsType, const char16_t*, const char16_t*) method


Configures the "Show Values As" calculation for this data field.

```cpp
void Aspose::Cells::Pivot::PivotField::ShowValuesAs(PivotShowValuesAsType showValuesAsType, const char16_t *baseField, const char16_t *baseItem)
```


| Parameter | Type | Description |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | The calculation type for Show Values As. |
| baseField | const char16_t* | The name of the base field used in the calculation. |
| baseItem | const char16_t* | Caption of a regular pivot item. Also accepts reserved literal keywords: **(previous)** for the previous item, **(next)** for the next item. Pass **null** if the selected calculation type does not require a base item. |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
