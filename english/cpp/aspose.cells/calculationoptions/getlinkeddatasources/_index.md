﻿---
title: Aspose::Cells::CalculationOptions::GetLinkedDataSources method
linktitle: GetLinkedDataSources
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::CalculationOptions::GetLinkedDataSources method. Specifies the data sources for external links used in formulas in C++.'
type: docs
weight: 1600
url: /cpp/aspose.cells/calculationoptions/getlinkeddatasources/
---
## CalculationOptions::GetLinkedDataSources method


Specifies the data sources for external links used in formulas.

```cpp
Vector<Workbook> Aspose::Cells::CalculationOptions::GetLinkedDataSources()
```

## Remarks


Like Workbook.UpdateLinkedDataSource(Workbook[]), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by Workbook.UpdateLinkedDataSource(Workbook[]). The match of those workbooks with external links is determined by Workbook.FileName and ExternalLink.DataSource. So please make sure Workbook.FileName has been specified with the proper value(generally it should be same with corresponding ExternalLink.DataSource) for every workbook so they can be linked as expected. 
## See Also

* Class [Vector](../../vector/)
* Class [Workbook](../../workbook/)
* Class [CalculationOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
