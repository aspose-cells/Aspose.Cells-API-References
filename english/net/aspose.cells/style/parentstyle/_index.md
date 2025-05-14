---
title: Style.ParentStyle
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets the parent style of this style
type: docs
url: /net/aspose.cells/style/parentstyle/
---
## Style.ParentStyle property

Gets the parent style of this style.

```csharp
public Style ParentStyle { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("base format s31", style.ParentStyle.Name);
public void Style_Property_ParentStyle()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xml");
    Assert.AreEqual(10, workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Size);
         
    workbook.Save(Constants.destPath + "dest.xlsx");
     workbook = new Workbook(Constants.sourcePath + "example.xml");
    Assert.AreEqual(10, workbook.Worksheets[0].Cells["A7"].GetStyle().Font.Size);
    Style style = workbook.Worksheets[1].Cells["A1"].GetStyle();
    Assert.AreEqual(20, style.Font.Size);
    Assert.AreEqual("base format s31", style.ParentStyle.Name);
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


