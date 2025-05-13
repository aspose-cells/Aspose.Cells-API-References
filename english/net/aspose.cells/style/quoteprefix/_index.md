---
title: Style.QuotePrefix
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicates whether the cells value starts with single quote mark
type: docs
url: /net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Indicates whether the cell's value starts with single quote mark.

```csharp
public bool QuotePrefix { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workBook.Worksheets[0].Cells["B10"].GetStyle().QuotePrefix);
public void Style_Property_QuotePrefix()
{

    var workBook = new Workbook(Constants.sourcePath + "example.xml");
    // workBook.Worksheets[0].Charts.Clear();
    Assert.IsTrue(workBook.Worksheets[0].Cells["B10"].GetStyle().QuotePrefix);
    workBook.Save(Constants.destPath + "example.xml");
    workBook = new Workbook(Constants.destPath + "example.xml");
    Assert.IsTrue(workBook.Worksheets[0].Cells["B10"].GetStyle().QuotePrefix);
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


