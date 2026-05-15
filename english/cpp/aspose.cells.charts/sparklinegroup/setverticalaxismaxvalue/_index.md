---
title: Aspose::Cells::Charts::SparklineGroup::SetVerticalAxisMaxValue method
linktitle: SetVerticalAxisMaxValue
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::SparklineGroup::SetVerticalAxisMaxValue method. Gets and sets the custom maximum value for the vertical axis in C++.'
type: docs
weight: 5500
url: /cpp/aspose.cells.charts/sparklinegroup/setverticalaxismaxvalue/
---
## SparklineGroup::SetVerticalAxisMaxValue(double) method


Gets and sets the custom maximum value for the vertical axis.

```cpp
void Aspose::Cells::Charts::SparklineGroup::SetVerticalAxisMaxValue(double value)
```

## Remarks


If this property is set, VerticalAxisMaxValueType will be [SparklineAxisMinMaxType.Custom](../../sparklineaxisminmaxtype/). 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SparklineGroup](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## SparklineGroup::SetVerticalAxisMaxValue(SparklineAxisMinMaxType, double) method


Sets the custom maximum value for the sparkline vertical axis with the specified axis value type.

```cpp
void Aspose::Cells::Charts::SparklineGroup::SetVerticalAxisMaxValue(SparklineAxisMinMaxType type, double value)
```


| Parameter | Type | Description |
| --- | --- | --- |
| type | SparklineAxisMinMaxType | Type that specifies how the axis maximum value is applied. |
| value | double | Custom maximum value of the vertical axis. Ignored if type is not [SparklineAxisMinMaxType.Custom](../../sparklineaxisminmaxtype/) |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* Class [SparklineGroup](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
