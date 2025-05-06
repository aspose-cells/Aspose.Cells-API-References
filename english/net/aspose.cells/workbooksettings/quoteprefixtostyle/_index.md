---
title: WorkbookSettings.QuotePrefixToStyle
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether setting QuotePrefix property when entering the string valuewhich starts with single quote mark  to the cell
type: docs
url: /net/aspose.cells/workbooksettings/quoteprefixtostyle/
---
## WorkbookSettings.QuotePrefixToStyle property

Indicates whether setting [`QuotePrefix`](../../style/quoteprefix/) property when entering the string value(which starts with single quote mark ) to the cell

```csharp
public bool QuotePrefixToStyle { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.QuotePrefixToStyle = true;
[Test] 
        public void Property_QuotePrefixToStyle()
        {

            Workbook workbook = new Workbook();
            workbook.Settings.QuotePrefixToStyle = true;
            Cell cell = workbook.Worksheets[0].Cells[&quot;A1&quot;];
            cell.PutValue(&quot;&apos;abc&quot;);
            Assert.IsTrue(cell.GetStyle().QuotePrefix);
            Assert.AreEqual(&quot;abc&quot;, cell.StringValue);
            workbook.Settings.QuotePrefixToStyle = false;
            cell = workbook.Worksheets[0].Cells[&quot;A2&quot;];
            cell.PutValue(&quot;&apos;abc&quot;);
            Assert.IsFalse(cell.GetStyle().QuotePrefix);
            Assert.AreEqual(&quot;&apos;abc&quot;, cell.StringValue);
            workbook.Save(Constants.destPath + &quot;CellsCore45.xlsx&quot;);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


