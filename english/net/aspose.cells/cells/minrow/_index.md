---
title: Cells.MinRow
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Minimum row index of cell which contains data or style
type: docs
url: /net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

Minimum row index of cell which contains data or style.

```csharp
public int MinRow { get; }
```

### Examples

```csharp
// Called: cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);
public void Cells_Property_MinRow()
{
    string path = Constants.sourcePath + "Charts/";
    var workbook = new Workbook(path + "example.xlsx");
    var ws = workbook.Worksheets[1];
    Cells cells = ws.Cells;
    cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);
    workbook.Save(Constants.destPath + "example.xlsx");
    var newWorkbook = new Workbook(Constants.destPath + "example.xlsx"); // reopen the saved xlsx
    newWorkbook.Worksheets[1].Cells["E4"].PutValue("CELLSNET49179"); // apply the text to the referenced cell
    //newWorkbook.Worksheets[1].Cells["C4"].PutValue("test2");
    //newWorkbook.Save(path + "out.xlsx"); // axis title missing
    Aspose.Cells.Charts.Chart chart1 = newWorkbook.Worksheets[0].Charts[0];
    string _linkedSource = chart1.ValueAxis.Title.LinkedSource;
    Assert.AreEqual("=Sheet1!$E$4", _linkedSource);
    string _title = chart1.ValueAxis.Title.Text;
    Assert.AreEqual("CELLSNET49179", _title);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


