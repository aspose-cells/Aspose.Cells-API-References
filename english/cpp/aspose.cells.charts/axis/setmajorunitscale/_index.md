---
title: Aspose::Cells::Charts::Axis::SetMajorUnitScale method
linktitle: SetMajorUnitScale
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Axis::SetMajorUnitScale method. Represents the major unit scale for the category axis in C++.'
type: docs
weight: 6400
url: /cpp/aspose.cells.charts/axis/setmajorunitscale/
---
## Axis::SetMajorUnitScale method


Represents the major unit scale for the category axis.

```cpp
void Aspose::Cells::Charts::Axis::SetMajorUnitScale(TimeUnit value)
```


## Examples


```cpp
chart.GetCategoryAxis().SetCategoryType(CategoryType::TimeScale);
TimeUnit majorUnitScale = chart.GetCategoryAxis().GetMajorUnitScale(); //get
chart.GetCategoryAxis().SetMajorUnitScale(majorUnitScale); //set
chart.GetCategoryAxis().SetMajorUnit(2);
```

## See Also

* Enum [TimeUnit](../../timeunit/)
* Class [Axis](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
