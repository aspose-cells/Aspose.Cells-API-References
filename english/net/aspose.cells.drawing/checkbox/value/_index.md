---
title: CheckBox.Value
second_title: Aspose.Cells for .NET API Reference
description: CheckBox property. Indicates if the checkbox is checked or not
type: docs
url: /net/aspose.cells.drawing/checkbox/value/
---
## CheckBox.Value property

Indicates if the checkbox is checked or not.

```csharp
public bool Value { get; set; }
```

### Examples

```csharp
// Called: cb.Value = true;
[Test]
        public void Property_Value()
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

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


