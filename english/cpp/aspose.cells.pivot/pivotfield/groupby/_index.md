---
title: Aspose::Cells::Pivot::PivotField::GroupBy method
linktitle: GroupBy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotField::GroupBy method. Automatically group the field with internal in C++.'
type: docs
weight: 1100
url: /cpp/aspose.cells.pivot/pivotfield/groupby/
---
## PivotField::GroupBy(double, bool) method


Automatically group the field with internal.

```cpp
void Aspose::Cells::Pivot::PivotField::GroupBy(double interval, bool newField)
```


| Parameter | Type | Description |
| --- | --- | --- |
| interval | double | The internal of group. Automatic value will be assigned if it's zero, |
| newField | bool | Indicates whether adding a new field to the pivottable. |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::GroupBy(const Vector \<PivotGroupByType\>\&, double, bool) method


Automatically group the field with internal.

```cpp
void Aspose::Cells::Pivot::PivotField::GroupBy(const Vector<PivotGroupByType> &groups, double interval, bool newField)
```


| Parameter | Type | Description |
| --- | --- | --- |
| groups | const Vector \<PivotGroupByType\>\& | Group types |
| interval | double | The internal of group. Automatic value will be assigned if it's zero, |
| newField | bool | Indicates whether adding a new field to the pivottable. |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotGroupByType](../../pivotgroupbytype/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::GroupBy(const Date\&, const Date\&, const Vector \<PivotGroupByType\>\&, double, bool) method


Group the file by the date group types.

```cpp
bool Aspose::Cells::Pivot::PivotField::GroupBy(const Date &start, const Date &end, const Vector<PivotGroupByType> &groups, double interval, bool firstAsNewField)
```


| Parameter | Type | Description |
| --- | --- | --- |
| start | const Date\& | The start datetime |
| end | const Date\& | The end of datetime |
| groups | const Vector \<PivotGroupByType\>\& | Group types |
| interval | double | The interval |
| firstAsNewField | bool | Indicates whether adding a new field to the pivottable. Only for the first group item. |

## ReturnValue

False means this field could not be grouped by date time.

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotGroupByType](../../pivotgroupbytype/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::GroupBy(bool, const Date\&, bool, const Date\&, const Vector \<PivotGroupByType\>\&, double, bool) method


Group the file by the date group types.

```cpp
bool Aspose::Cells::Pivot::PivotField::GroupBy(bool isAutoStart, const Date &start, bool isAutoEnd, const Date &end, const Vector<PivotGroupByType> &groups, double interval, bool firstAsNewField)
```


| Parameter | Type | Description |
| --- | --- | --- |
| isAutoStart | bool | Indicates whether to auto detect the start date time value. |
| start | const Date\& | The start datetime |
| isAutoEnd | bool | Indicates whether to auto detect the end date time value. |
| end | const Date\& | The end of datetime |
| groups | const Vector \<PivotGroupByType\>\& | Group types |
| interval | double | The interval |
| firstAsNewField | bool | Indicates whether adding a new field to the pivottable. Only for the first group item. |

## ReturnValue

False means this field could not be grouped by date time.

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotGroupByType](../../pivotgroupbytype/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::GroupBy(double, double, double, bool) method


Group the file by number.

```cpp
bool Aspose::Cells::Pivot::PivotField::GroupBy(double start, double end, double interval, bool newField)
```


| Parameter | Type | Description |
| --- | --- | --- |
| start | double | The start value |
| end | double | The end of value |
| interval | double | The interval |
| newField | bool | Indicates whether adding a new field to the pivottable |

## ReturnValue

False means this field could not be grouped by date time.

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::GroupBy(bool, double, bool, double, double, bool) method


Group the file by number.

```cpp
bool Aspose::Cells::Pivot::PivotField::GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, bool newField)
```


| Parameter | Type | Description |
| --- | --- | --- |
| isAutoStart | bool | Indicates whether to auto detect the start value. |
| start | double | The start value |
| isAutoEnd | bool | Indicates whether to auto detect the end value. |
| end | double | The end of value |
| interval | double | The interval |
| newField | bool | Indicates whether adding a new field to the pivottable |

## ReturnValue

False means this field could not be grouped by date time.

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::GroupBy(const Vector \<CustomPiovtFieldGroupItem\>\&, bool) method


Custom group the field.

```cpp
bool Aspose::Cells::Pivot::PivotField::GroupBy(const Vector<CustomPiovtFieldGroupItem> &customGroupItems, bool newField)
```


| Parameter | Type | Description |
| --- | --- | --- |
| customGroupItems | const Vector \<CustomPiovtFieldGroupItem\>\& | The custom group items. |
| newField | bool | Indicates whether adding a new field to the pivottable |

## ReturnValue

False means this field could not be grouped by date time.

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
