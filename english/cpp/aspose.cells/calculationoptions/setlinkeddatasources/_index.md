---
title: Aspose::Cells::CalculationOptions::SetLinkedDataSources method
linktitle: SetLinkedDataSources
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::CalculationOptions::SetLinkedDataSources method. Specifies the data sources for external links used in formulas in C++.'
type: docs
weight: 1700
url: /cpp/aspose.cells/calculationoptions/setlinkeddatasources/
---
## CalculationOptions::SetLinkedDataSources method


Specifies the data sources for external links used in formulas.

```cpp
void Aspose::Cells::CalculationOptions::SetLinkedDataSources(const Vector<Workbook> &value)
```

## Remarks


Like Workbook.UpdateLinkedDataSource(Workbook[]), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by Workbook.UpdateLinkedDataSource(Workbook[]). 
## See Also

* Class [Vector](../../vector/)
* Class [Workbook](../../workbook/)
* Class [CalculationOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
