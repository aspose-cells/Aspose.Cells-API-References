---
title: FillFormat.FillType
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Gets and sets fill type
type: docs
url: /net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

Gets and sets fill type

```csharp
public FillType FillType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(FillType.None, shape.Fill.FillType);
public void FillFormat_Property_FillType()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xls");
    Shape shape = workbook.Worksheets[1].Shapes["AutoShape 164"];
    Console.WriteLine(shape.Text);
   Assert.AreEqual(FillType.None, shape.Fill.FillType);
   workbook.Save(Constants.destPath + "example.pdf");
}
```

### See Also

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


