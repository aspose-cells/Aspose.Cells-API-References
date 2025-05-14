---
title: TextOptions.FarEastName
second_title: Aspose.Cells for .NET API Reference
description: TextOptions property. Gets and sets the FarEast name
type: docs
url: /net/aspose.cells.drawing.texts/textoptions/fareastname/
---
## TextOptions.FarEastName property

Gets and sets the FarEast name.

```csharp
public string FarEastName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(shape.TextOptions.FarEastName, "宋体");
public void TextOptions_Property_FarEastName()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Shape shape = workbook.Worksheets[0].Shapes[0];

    shape.TextOptions.FarEastName = "宋体";
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    shape = workbook.Worksheets[0].Shapes[0];
    Assert.AreEqual(shape.TextOptions.FarEastName, "宋体");
}
```

### See Also

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


