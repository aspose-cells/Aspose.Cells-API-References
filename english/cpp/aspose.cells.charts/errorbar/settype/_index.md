---
title: Aspose::Cells::Charts::ErrorBar::SetType method
linktitle: SetType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ErrorBar::SetType method. Represents error bar amount type in C++.'
type: docs
weight: 700
url: /cpp/aspose.cells.charts/errorbar/settype/
---
## ErrorBar::SetType method


Represents error bar amount type.

```cpp
void Aspose::Cells::Charts::ErrorBar::SetType(ErrorBarType value)
```


## Examples


```cpp
Aspose::Cells::Startup();
Workbook wb(u"chart.xlsx");
Chart chart = wb.GetWorksheets().Get(0).GetCharts().Get(0);
Series aseries = chart.GetNSeries().Get(0);
//Sets custom error bar type
aseries.GetYErrorBar().SetType(ErrorBarType::Custom);
aseries.GetYErrorBar().SetPlusValue(u"=Sheet1!A1");
aseries.GetYErrorBar().SetMinusValue(u"=Sheet1!A2");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [ErrorBarType](../../errorbartype/)
* Class [ErrorBar](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
