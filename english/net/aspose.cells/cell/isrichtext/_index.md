---
title: Cell.IsRichText
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Indicates whether the string value of this cell is a rich formatted text
type: docs
url: /net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Indicates whether the string value of this cell is a rich formatted text.

```csharp
public bool IsRichText()
```

### Examples

```csharp
// Called: Assert.AreEqual(a1.IsRichText(), true);
public void Cell_Method_IsRichText()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45035/";
    var wb = new Workbook(filePath + "sample.html");
    Cell a1 = wb.Worksheets[0].Cells["A1"];
    Assert.AreEqual(a1.IsRichText(), true);
    Assert.AreEqual(a1.GetCharacters()[0].Font.IsBold, true);
    Assert.AreEqual(a1.GetCharacters()[1].Font.IsBold, false);
    wb.Save(CreateFolder(filePath) + "out.xlsx", SaveFormat.Xlsx);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


