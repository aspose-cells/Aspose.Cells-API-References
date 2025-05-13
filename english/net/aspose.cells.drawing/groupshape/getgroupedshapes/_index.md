---
title: GroupShape.GetGroupedShapes
second_title: Aspose.Cells for .NET API Reference
description: GroupShape method. Gets the shapes grouped by this shape
type: docs
url: /net/aspose.cells.drawing/groupshape/getgroupedshapes/
---
## GroupShape.GetGroupedShapes method

Gets the shapes grouped by this shape.

```csharp
public Shape[] GetGroupedShapes()
```

### Examples

```csharp
// Called: Shape[] groupedShapes = resultOfSmartArt.GetGroupedShapes();
public void GroupShape_Method_GetGroupedShapes()
{
    Workbook workbook = new Workbook(Constants.sourcePath+ "example.xlsx");
     GroupShape resultOfSmartArt = workbook.Worksheets[0].Shapes[0].GetResultOfSmartArt();
    Shape[] groupedShapes = resultOfSmartArt.GetGroupedShapes();
    Assert.AreEqual("AlternativeText(Description)" ,groupedShapes[0].AlternativeText);
    Util.ReSave(workbook, SaveFormat.Xlsx);
    //workbook.Save(Constants.destPath +"example.xlsx");
}
```

### See Also

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


