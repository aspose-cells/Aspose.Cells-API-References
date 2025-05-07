---
title: PivotArea.OnlyLabel
second_title: Aspose.Cells for .NET API Reference
description: PivotArea property. Indicates whether only the data labels for an item selection are selected
type: docs
url: /net/aspose.cells.pivot/pivotarea/onlylabel/
---
## PivotArea.OnlyLabel property

Indicates whether only the data labels for an item selection are selected.

```csharp
public bool OnlyLabel { get; set; }
```

### Examples

```csharp
// Called: pt.PivotFormats[0].PivotArea.OnlyLabel = true;//onlydata = false
[Test]
        public void Property_OnlyLabel()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET56640.xlsx");

            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;
            //onlydata is true, onlylabel = false
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(193, 229, 245), cells["G6"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(193, 229, 245), cells["G9"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["G10"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["G13"].GetStyle().ForegroundColor));
            //G6 G9 G10 G13
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.PivotFormats[0].PivotArea.OnlyData = false;//onlylabel = false
            workbook.Worksheets.RefreshAll();
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["G6"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["G9"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["G10"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["G13"].GetStyle().ForegroundColor));

            pt.PivotFormats[0].PivotArea.OnlyLabel = true;//onlydata = false
            workbook.Worksheets.RefreshAll();
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["G6"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["G9"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Empty, cells["G10"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(193, 229, 245), cells["G13"].GetStyle().ForegroundColor));
            workbook.Save(Constants.PivotTableDestPath + "CELLSNET56640.html");
        }
```

### See Also

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


