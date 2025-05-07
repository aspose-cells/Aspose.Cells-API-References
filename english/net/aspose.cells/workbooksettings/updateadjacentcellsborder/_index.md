---
title: WorkbookSettings.UpdateAdjacentCellsBorder
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether update adjacent cells border
type: docs
url: /net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

Indicates whether update adjacent cells' border.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### Remarks

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

### Examples

```csharp
// Called: workbook.Settings.UpdateAdjacentCellsBorder = true;
[Test]
        public void Property_UpdateAdjacentCellsBorder()
        {
            var workbook = new Workbook(Constants.sourcePath + "CellsNet43293.xlsx");
            var ws = workbook.Worksheets[0];

            var rng = ws.Cells.CreateRange("B13:J13");


            rng.SetOutlineBorder(BorderType.TopBorder, CellBorderType.None, System.Drawing.Color.Empty);

            Assert.AreEqual(ws.Cells["B13"].GetStyle(true).Borders[BorderType.TopBorder].LineStyle, CellBorderType.None);
          
            workbook = new Workbook(Constants.sourcePath + "CellsNet43293.xlsx");
            workbook.Settings.UpdateAdjacentCellsBorder = true;
             ws = workbook.Worksheets[0];

             Style style = workbook.CreateStyle();

             style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;

             StyleFlag flag = new StyleFlag();

             //flag.TopBorder = true;

             flag.All = true;

             rng = ws.Cells.CreateRange("B13:J13");
             rng.ApplyStyle(style, flag);
             Assert.AreEqual(ws.Cells["B13"].GetStyle(true).Borders[BorderType.TopBorder].LineStyle, CellBorderType.None);

        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


