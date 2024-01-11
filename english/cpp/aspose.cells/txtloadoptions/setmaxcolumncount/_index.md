---
title: Aspose::Cells::TxtLoadOptions::SetMaxColumnCount method
linktitle: SetMaxColumnCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::TxtLoadOptions::SetMaxColumnCount method. The maximum count of columns to be imported for one sheet in C++.'
type: docs
weight: 3100
url: /cpp/aspose.cells/txtloadoptions/setmaxcolumncount/
---
## TxtLoadOptions::SetMaxColumnCount method


The maximum count of columns to be imported for one sheet.

```cpp
void Aspose::Cells::TxtLoadOptions::SetMaxColumnCount(int32_t value)
```

## Remarks


Those columns exceeding this limit will be ignored or extended to next sheet according to ExtendToNextSheet. This count includes the header columns(HeaderColumnsCount). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
## See Also

* Class [Vector](../../vector/)
* Class [TxtLoadOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
