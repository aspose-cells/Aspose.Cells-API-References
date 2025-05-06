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
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Workbook wb = new Workbook();
            wb.Worksheets.Clear();
            int i = wb.Worksheets.Add();
            var ws = wb.Worksheets[i];
            ws.Name = &quot;New&quot;;


            var index = ws.CheckBoxes.Add(10, 2, 20, ws.Cells.GetColumnWidthPixel(1) + ws.Cells.GetColumnWidthPixel(3) - 5);


            Aspose.Cells.Drawing.CheckBox cb = ws.CheckBoxes[index];
            cb.Text = &quot;Location 1 ([%¤#!#%&amp;!§§!#¤HELLO)&quot;;
            cb.Font.Size = 10;
            cb.TextVerticalAlignment = TextAlignmentType.Center;
            var hideCell = &quot;B&quot; + (10 + 1).ToString();
            ws.Cells[hideCell].PutValue(&quot;LnkCell&quot;);
            cb.LinkedCell = hideCell;
            cb.Value = true;
            cb.LineFormat.ForeColor = Color.Orange;
            cb.LineFormat.Style = Aspose.Cells.Drawing.MsoLineStyle.Single;
            cb.LineFormat.Weight = 2;


            wb.Save(Constants.destPath + &quot;Result.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


