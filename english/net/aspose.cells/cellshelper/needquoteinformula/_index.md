---
title: CellsHelper.NeedQuoteInFormula
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Indicates whether the name of the sheet should be enclosed in single quotes
type: docs
url: /net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

Indicates whether the name of the sheet should be enclosed in single quotes

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | The name of the sheet |

### Examples

```csharp
// Called: Assert.IsTrue(CellsHelper.NeedQuoteInFormula("A123"));
public void CellsHelper_Method_NeedQuoteInFormula()
{
    Assert.IsTrue(CellsHelper.NeedQuoteInFormula("Test Ab"));
    Assert.IsTrue(CellsHelper.NeedQuoteInFormula("A123"));
    Assert.IsFalse(CellsHelper.NeedQuoteInFormula("Sheet1"));
}
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


