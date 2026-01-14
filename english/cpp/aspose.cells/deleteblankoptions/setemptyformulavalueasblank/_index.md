---
title: Aspose::Cells::DeleteBlankOptions::SetEmptyFormulaValueAsBlank method
linktitle: SetEmptyFormulaValueAsBlank
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DeleteBlankOptions::SetEmptyFormulaValueAsBlank method. Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false in C++.'
type: docs
weight: 900
url: /cpp/aspose.cells/deleteblankoptions/setemptyformulavalueasblank/
---
## DeleteBlankOptions::SetEmptyFormulaValueAsBlank method


Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false.

```cpp
void Aspose::Cells::DeleteBlankOptions::SetEmptyFormulaValueAsBlank(bool value)
```

## Remarks


Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as Cell.Formula will be taken as blank and may be deleted because before calculation their calculated results are all null. 
## See Also

* Class [Vector](../../vector/)
* Class [DeleteBlankOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
