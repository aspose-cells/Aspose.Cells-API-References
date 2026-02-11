---
title: Aspose::Cells::Charts::SparklineGroupCollection::Add method
linktitle: Add
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::SparklineGroupCollection::Add method. Adds an SparklineGroup with a Sparkline to the collection in C++.'
type: docs
weight: 700
url: /cpp/aspose.cells.charts/sparklinegroupcollection/add/
---
## SparklineGroupCollection::Add(SparklineType) method


Adds an [SparklineGroup](../../sparklinegroup/) with a [Sparkline](../../sparkline/) to the collection.

```cpp
int32_t Aspose::Cells::Charts::SparklineGroupCollection::Add(SparklineType type)
```


| Parameter | Type | Description |
| --- | --- | --- |
| type | SparklineType | Specifies the type of the [Sparkline](../../sparkline/) group. |

## ReturnValue

[SparklineGroup](../../sparklinegroup/) object index.

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [SparklineType](../../sparklinetype/)
* Class [SparklineGroupCollection](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## SparklineGroupCollection::Add(SparklineType, const U16String\&, bool, const CellArea\&) method


Adds an [SparklineGroup](../../sparklinegroup/) with some [Sparkline](../../sparkline/) to the collection.

```cpp
int32_t Aspose::Cells::Charts::SparklineGroupCollection::Add(SparklineType type, const U16String &dataRange, bool isVertical, const CellArea &locationRange)
```


| Parameter | Type | Description |
| --- | --- | --- |
| type | SparklineType | Specifies the type of the [Sparkline](../../sparkline/) group. |
| dataRange | const U16String\& | Specifies the data range of the sparkline group. |
| isVertical | bool | Specifies whether to plot the sparklines from the data range by row or by column. |
| locationRange | const CellArea\& | Specifies where the sparklines to be placed. |

## ReturnValue

[SparklineGroup](../../sparklinegroup/) object index.
## Remarks



This method will create sparklines too. If *isVertical*  is true, the number of rows in dataRange and locationRange must be same. If *isVertical*  is false, the number of columns in dataRange and locationRange must be same. 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [SparklineType](../../sparklinetype/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [CellArea](../../../aspose.cells/cellarea/)
* Class [SparklineGroupCollection](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## SparklineGroupCollection::Add(SparklineType, const char16_t*, bool, const CellArea\&) method


Adds an [SparklineGroup](../../sparklinegroup/) with some [Sparkline](../../sparkline/) to the collection.

```cpp
int32_t Aspose::Cells::Charts::SparklineGroupCollection::Add(SparklineType type, const char16_t *dataRange, bool isVertical, const CellArea &locationRange)
```


| Parameter | Type | Description |
| --- | --- | --- |
| type | SparklineType | Specifies the type of the [Sparkline](../../sparkline/) group. |
| dataRange | const char16_t* | Specifies the data range of the sparkline group. |
| isVertical | bool | Specifies whether to plot the sparklines from the data range by row or by column. |
| locationRange | const CellArea\& | Specifies where the sparklines to be placed. |

## ReturnValue

[SparklineGroup](../../sparklinegroup/) object index.
## Remarks



This method will create sparklines too. If *isVertical*  is true, the number of rows in dataRange and locationRange must be same. If *isVertical*  is false, the number of columns in dataRange and locationRange must be same. 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [SparklineType](../../sparklinetype/)
* Class [CellArea](../../../aspose.cells/cellarea/)
* Class [SparklineGroupCollection](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
