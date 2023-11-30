---
title: Aspose::Cells::Charts::ErrorBar::GetType method
linktitle: GetType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ErrorBar::GetType method. Represents error bar amount type in C++.'
type: docs
weight: 600
url: /cpp/aspose.cells.charts/errorbar/gettype/
---
## ErrorBar::GetType method


Represents error bar amount type.

```cpp
ErrorBarType Aspose::Cells::Charts::ErrorBar::GetType()
```


## Examples


```cpp
Aspose::Cells::Startup();
Workbook wb(u"chart.xlsx");
Chart chart = wb.GetWorksheets().Get(0).GetCharts().Get(0);
Series aseries = chart.GetNSeries().Get(0);
//Sets custom error bar type
ErrorBarType ty = aseries.GetYErrorBar().GetType();
Aspose::Cells::Cleanup();
```

## See Also

* Enum [ErrorBarType](../../errorbartype/)
* Class [ErrorBar](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
