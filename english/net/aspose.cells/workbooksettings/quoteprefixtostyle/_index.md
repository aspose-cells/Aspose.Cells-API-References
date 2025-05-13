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
// Called: workbook.Settings.QuotePrefixToStyle = false;
public void WorkbookSettings_Property_QuotePrefixToStyle()
{

    Workbook workbook = new Workbook();
    workbook.Settings.QuotePrefixToStyle = true;
    Cell cell = workbook.Worksheets[0].Cells["A1"];
    cell.PutValue("'abc");
    Assert.IsTrue(cell.GetStyle().QuotePrefix);
    Assert.AreEqual("abc", cell.StringValue);
    workbook.Settings.QuotePrefixToStyle = false;
    cell = workbook.Worksheets[0].Cells["A2"];
    cell.PutValue("'abc");
    Assert.IsFalse(cell.GetStyle().QuotePrefix);
    Assert.AreEqual("'abc", cell.StringValue);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


