---
title: CheckBoxCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: CheckBoxCollection method. Adds a checkBox to the collection
type: docs
url: /net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

Adds a checkBox to the collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| height | Int32 | Height of checkBox, in unit of pixel. |
| width | Int32 | Width of checkBox, in unit of pixel. |

### Return Value

[`CheckBox`](../../checkbox/) object index.

### Examples

```csharp
// Called: var index = ws.CheckBoxes.Add(10, 2, 20, ws.Cells.GetColumnWidthPixel(1) + ws.Cells.GetColumnWidthPixel(3) - 5);
public void CheckBoxCollection_Method_Add()
{
    Workbook workbook = new Workbook();
    Workbook wb = new Workbook();
    wb.Worksheets.Clear();
    int i = wb.Worksheets.Add();
    var ws = wb.Worksheets[i];
    ws.Name = "New";


    var index = ws.CheckBoxes.Add(10, 2, 20, ws.Cells.GetColumnWidthPixel(1) + ws.Cells.GetColumnWidthPixel(3) - 5);


    Aspose.Cells.Drawing.CheckBox cb = ws.CheckBoxes[index];
    cb.Text = "Location 1 ([%¤#!#%&!§§!#¤HELLO)";
    cb.Font.Size = 10;
    cb.TextVerticalAlignment = TextAlignmentType.Center;
    var hideCell = "B" + (10 + 1).ToString();
    ws.Cells[hideCell].PutValue("LnkCell");
    cb.LinkedCell = hideCell;
    cb.Value = true;
    cb.LineFormat.ForeColor = Color.Orange;
    cb.LineFormat.Style = Aspose.Cells.Drawing.MsoLineStyle.Single;
    cb.LineFormat.Weight = 2;


    wb.Save(Constants.destPath + "Result.xlsx", SaveFormat.Xlsx);
}
```

### See Also

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


