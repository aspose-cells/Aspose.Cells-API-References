---
title: Aspose::Cells::ReferredArea::GetSheetName method
linktitle: GetSheetName
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ReferredArea::GetSheetName method. Indicates which sheet this reference is in in C++.'
type: docs
weight: 800
url: /cpp/aspose.cells/referredarea/getsheetname/
---
## ReferredArea::GetSheetName method


Indicates which sheet this reference is in.

```cpp
U16String Aspose::Cells::ReferredArea::GetSheetName()
```

## Remarks


If it references to multiple worksheets, the returned value is just like the range expression in the formula. For example "Sheet1:Sheet3" for the reference in formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)". 
## See Also

* Class [U16String](../../u16string/)
* Class [ReferredArea](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
