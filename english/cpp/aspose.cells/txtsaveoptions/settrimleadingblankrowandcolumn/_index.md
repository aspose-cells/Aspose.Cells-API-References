﻿---
title: Aspose::Cells::TxtSaveOptions::SetTrimLeadingBlankRowAndColumn method
linktitle: SetTrimLeadingBlankRowAndColumn
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::TxtSaveOptions::SetTrimLeadingBlankRowAndColumn method. Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true in C++.'
type: docs
weight: 1900
url: /cpp/aspose.cells/txtsaveoptions/settrimleadingblankrowandcolumn/
---
## TxtSaveOptions::SetTrimLeadingBlankRowAndColumn method


Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true.

```cpp
void Aspose::Cells::TxtSaveOptions::SetTrimLeadingBlankRowAndColumn(bool value)
```

## Remarks


Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [LightCellsDataProvider](../../lightcellsdataprovider/) or by speicifing ExportArea 
## See Also

* Class [Vector](../../vector/)
* Class [TxtSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
