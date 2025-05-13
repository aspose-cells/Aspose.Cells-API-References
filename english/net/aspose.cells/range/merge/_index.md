---
title: Range.Merge
second_title: Aspose.Cells for .NET API Reference
description: Range method. Combines a range of cells into a single cell
type: docs
url: /net/aspose.cells/range/merge/
---
## Range.Merge method

Combines a range of cells into a single cell.

```csharp
public void Merge()
```

### Remarks

Reference the merged cell via the address of the upper-left cell in the range.

### Examples

```csharp
// Called: sheet.Cells.CreateRange(0, 0, 1, 2).Merge();
public void Range_Method_Merge()
{
    Workbook wb = new Workbook();
    var sheet = wb.Worksheets[0];
    //create 2x1 merge cell
    sheet.Cells.CreateRange(0, 0, 1, 2).Merge();
    sheet.Cells[0, 0].Value = "&=obj.Property(group:merge)";
    sheet.Cells[0, 2].Value = "&=obj.AABB";
    //output template file
   // const string templateFile = "template.xlsx";
    //    wb.Save(templateFile);
    //   Process.Start("cmd", $"/c start {templateFile}");
    var designer = new WorkbookDesigner(wb);
    designer.SetDataSource("obj", new[] { new objClass("Value1", "Value2"), new objClass("Value1", "Value2"), new objClass("Value1", "Value3"), new objClass("Value1", "Value4"), new objClass("Value2", "Value2") });
    designer.Process();
    CellArea ca = (CellArea)wb.Worksheets[0].Cells.GetMergedAreas()[0];
    Assert.AreEqual(3, ca.EndRow);

    wb.Save(Constants.destPath + @"example.xlsx");
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


