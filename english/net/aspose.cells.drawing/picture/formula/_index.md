---
title: Picture.Formula
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets and sets the data of the formula
type: docs
url: /net/aspose.cells.drawing/picture/formula/
---
## Picture.Formula property

Gets and sets the data of the formula.

```csharp
public string Formula { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("=A1:A3", workbook.Worksheets[0].Pictures[0].Formula);
public void Picture_Property_Formula()
{
    Workbook workbook = new Workbook();
    Picture picture = workbook.Worksheets[0].Pictures[workbook.Worksheets[0].Pictures.Add(0, 0, Constants.sourcePath + "example.jpg")];
    picture.Formula = "A1:A3";
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual("=A1:A3", workbook.Worksheets[0].Pictures[0].Formula);

    workbook.Worksheets[0].Pictures[0].Formula = "B1:B3";
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual("=B1:B3", workbook.Worksheets[0].Pictures[0].Formula);
}
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


