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
// Called: Assert.IsFalse(CellsHelper.NeedQuoteInFormula(&amp;quot;My.Test&amp;quot;));
[Test]
        public void Method_String_()
        {
            Assert.IsFalse(CellsHelper.NeedQuoteInFormula(&quot;My.Test&quot;));
            Workbook wb = new Workbook();
            wb.Worksheets.Add(&quot;My.Test&quot;);
            NameCollection nc = wb.Worksheets.Names;
            Name n = nc[nc.Add(&quot;My.Test!TestName&quot;)];
            Assert.AreEqual(&quot;My.Test!TestName&quot;, n.FullText, &quot;FullText&quot;);
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


