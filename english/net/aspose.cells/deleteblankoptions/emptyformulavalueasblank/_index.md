---
title: DeleteBlankOptions.EmptyFormulaValueAsBlank
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false
type: docs
url: /net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Remarks

Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as [`Formula`](../../cell/formula/) will be taken as blank and may be deleted because before calculation their calculated results are all null.

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


