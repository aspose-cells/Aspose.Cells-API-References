﻿---
title: Aspose::Cells::TxtLoadOptions::GetMaxColumnCount method
linktitle: GetMaxColumnCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::TxtLoadOptions::GetMaxColumnCount method. The maximum count of columns to be imported for one sheet in C++.'
type: docs
weight: 3000
url: /cpp/aspose.cells/txtloadoptions/getmaxcolumncount/
---
## TxtLoadOptions::GetMaxColumnCount method


The maximum count of columns to be imported for one sheet.

```cpp
int32_t Aspose::Cells::TxtLoadOptions::GetMaxColumnCount()
```

## Remarks


Those columns exceeding this limit will be ignored or extended to next sheet according to ExtendToNextSheet. This count includes the header columns(HeaderColumnsCount). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
## See Also

* Class [Vector](../../vector/)
* Class [TxtLoadOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
