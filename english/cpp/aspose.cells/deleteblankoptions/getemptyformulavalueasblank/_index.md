---
title: Aspose::Cells::DeleteBlankOptions::GetEmptyFormulaValueAsBlank method
linktitle: GetEmptyFormulaValueAsBlank
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DeleteBlankOptions::GetEmptyFormulaValueAsBlank method. Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false in C++.'
type: docs
weight: 800
url: /cpp/aspose.cells/deleteblankoptions/getemptyformulavalueasblank/
---
## DeleteBlankOptions::GetEmptyFormulaValueAsBlank method


Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false.

```cpp
bool Aspose::Cells::DeleteBlankOptions::GetEmptyFormulaValueAsBlank()
```

## Remarks


Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as Cell.Formula will be taken as blank and may be deleted because before calculation their calculated results are all null. 
## See Also

* Class [Vector](../../vector/)
* Class [DeleteBlankOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
