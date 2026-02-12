---
title: Aspose::Cells::Charts::SeriesCollection::Add method
linktitle: Add
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::SeriesCollection::Add method. Adds the Series collection to a chart in C++.'
type: docs
weight: 1700
url: /cpp/aspose.cells.charts/seriescollection/add/
---
## SeriesCollection::Add(const U16String\&, bool) method


Adds the [Series](../../series/) collection to a chart.

```cpp
int32_t Aspose::Cells::Charts::SeriesCollection::Add(const U16String &dataArea, bool isVertical)
```


| Parameter | Type | Description |
| --- | --- | --- |
| dataArea | const U16String\& | Specifies values from which to plot the data series |
| isVertical | bool | Specifies whether to plot the series from a range of cell values by row or by column. If true, [Series](../../series/) will be added column by column |

## ReturnValue

Return the first index of the added ASeries in the NSeries.
## Remarks





If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5. 

If set data on non contiguous cells, use comma to seperate them.For example: ($C$2,$D$5). 

This method only simply process *dataArea*  as data range. If you want to smartly check [ChartCollection.Add()](../../chartcollection/add/) method.  
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SeriesCollection](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## SeriesCollection::Add(const char16_t*, bool) method


Adds the [Series](../../series/) collection to a chart.

```cpp
int32_t Aspose::Cells::Charts::SeriesCollection::Add(const char16_t *dataArea, bool isVertical)
```


| Parameter | Type | Description |
| --- | --- | --- |
| dataArea | const char16_t* | Specifies values from which to plot the data series |
| isVertical | bool | Specifies whether to plot the series from a range of cell values by row or by column. If true, [Series](../../series/) will be added column by column |

## ReturnValue

Return the first index of the added ASeries in the NSeries.
## Remarks





If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5. 

If set data on non contiguous cells, use comma to seperate them.For example: ($C$2,$D$5). 

This method only simply process *dataArea*  as data range. If you want to smartly check [ChartCollection.Add()](../../chartcollection/add/) method.  
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SeriesCollection](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## SeriesCollection::Add(const U16String\&, bool, bool) method


Adds the [Series](../../series/) collection to a chart.

```cpp
int32_t Aspose::Cells::Charts::SeriesCollection::Add(const U16String &area, bool isVertical, bool checkLabels)
```


| Parameter | Type | Description |
| --- | --- | --- |
| area | const U16String\& | Specifies values from which to plot the data series |
| isVertical | bool | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | bool | Indicates whether the range contains series's name |

## ReturnValue

Return the first index of the added ASeries in the NSeries.
## Remarks





If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5. 

If set data on non contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SeriesCollection](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## SeriesCollection::Add(const char16_t*, bool, bool) method


Adds the [Series](../../series/) collection to a chart.

```cpp
int32_t Aspose::Cells::Charts::SeriesCollection::Add(const char16_t *area, bool isVertical, bool checkLabels)
```


| Parameter | Type | Description |
| --- | --- | --- |
| area | const char16_t* | Specifies values from which to plot the data series |
| isVertical | bool | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | bool | Indicates whether the range contains series's name |

## ReturnValue

Return the first index of the added ASeries in the NSeries.
## Remarks





If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5. 

If set data on non contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SeriesCollection](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
