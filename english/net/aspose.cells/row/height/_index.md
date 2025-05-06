---
title: Row.Height
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets and sets the row height in unit of Points
type: docs
url: /net/aspose.cells/row/height/
---
## Row.Height property

Gets and sets the row height in unit of Points.

```csharp
public double Height { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(row.Height, 38.25);
[Test]
        public void Property_Height()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;
            Row row = cells.Rows[0];


            // Set the width of first column 
            cells.SetColumnWidth(0, 10);
            // Set wrap text option for cells 
            Style style = cells[0, 0].GetStyle();
            style.IsTextWrapped = (true);
            cells[0, 0].SetStyle(style);
            cells[0, 1].SetStyle(style);
            cells[0, 2].SetStyle(style);

            // Merge cells 
            cells.Merge(0, 1, 1, 2);



            cells[0, 0].PutValue(&quot;This is a autoFitRows call test&quot;);
            cells[1, 0].PutValue(&quot;This is a merged cells to test auto-fit in scope of hidden column&quot;);

            cells.HideColumn(0);

            // Apply auto-fit 
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = (true);
            options.AutoFitMergedCells = (false);
            options.IgnoreHidden = (false);
            worksheet.AutoFitRows(options);
            row = cells.Rows[0];
            Assert.AreEqual(row.Height, 38.25);
        }
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


