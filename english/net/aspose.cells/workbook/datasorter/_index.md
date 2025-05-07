---
title: Workbook.DataSorter
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets a DataSorter object to sort data
type: docs
url: /net/aspose.cells/workbook/datasorter/
---
## Workbook.DataSorter property

Gets a DataSorter object to sort data.

```csharp
public DataSorter DataSorter { get; }
```

### Examples

```csharp
// Called: wb.DataSorter.Key3 = wb.Worksheets[0].Cells["C2"].Column;
[Test]
        public void Property_DataSorter()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "Sort/CellsNet45421.xls");
            wb.CalculateFormula();

            wb.DataSorter.Order1 = SortOrder.Ascending;
            wb.DataSorter.Key1 = wb.Worksheets[0].Cells["D2"].Column;

            wb.DataSorter.Order2 = SortOrder.Ascending;
            wb.DataSorter.Key2 = wb.Worksheets[0].Cells["E2"].Column;

            wb.DataSorter.Order3 = SortOrder.Ascending;
            wb.DataSorter.Key3 = wb.Worksheets[0].Cells["C2"].Column;

            CellArea ca = new CellArea();
            ca.StartRow = 1;
            ca.StartColumn = 0;
            ca.EndRow = 10;
            ca.EndColumn = 9;

            wb.DataSorter.Sort(wb.Worksheets[0].Cells, ca);
            Assert.AreEqual("=F2/D2*7", wb.Worksheets[0].Cells["G2"].Formula);
            Assert.AreEqual("=F3/D3*7", wb.Worksheets[0].Cells["G3"].Formula);
        }
```

### See Also

* class [DataSorter](../../datasorter/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


