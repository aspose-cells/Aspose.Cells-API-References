---
title: Aspose::Cells::Charts::Axis::GetMajorUnitScale method
linktitle: GetMajorUnitScale
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Axis::GetMajorUnitScale method. Represents the major unit scale for the category axis in C++.'
type: docs
weight: 6300
url: /cpp/aspose.cells.charts/axis/getmajorunitscale/
---
## Axis::GetMajorUnitScale method


Represents the major unit scale for the category axis.

```cpp
TimeUnit Aspose::Cells::Charts::Axis::GetMajorUnitScale()
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
