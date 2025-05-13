---
title: CellArea.ToString
second_title: Aspose.Cells for .NET API Reference
description: CellArea method. Returns a string represents the current cell area object
type: docs
url: /net/aspose.cells/cellarea/tostring/
---
## CellArea.ToString method

Returns a string represents the current cell area object.

```csharp
public override string ToString()
```

### Examples

```csharp
// Called: Assert.AreEqual("Aspose.Cells.CellArea(C4:D6)[3,2,5,3]", ca.ToString());
public void CellArea_Method_ToString()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");

    CellArea[] areas = workbook.Worksheets[0].Cells.GetMergedAreas();
   Assert.AreEqual(3,areas.Length);
    CellArea ca = (CellArea)areas[0];
    Assert.AreEqual("Aspose.Cells.CellArea(C4:D6)[3,2,5,3]", ca.ToString());
    ca = (CellArea)areas[1];
    Assert.AreEqual("Aspose.Cells.CellArea(F9:G11)[8,5,10,6]", ca.ToString());
 
     ca = (CellArea)areas[2];
    Assert.AreEqual("Aspose.Cells.CellArea(C10:D15)[9,2,14,3]", ca.ToString());
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


