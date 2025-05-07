---
title: PivotTableRefreshOption.PivotTableRefreshOption
second_title: Aspose.Cells for .NET API Reference
description: PivotTableRefreshOption constructor. Represents the options of refreshing data source of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottablerefreshoption/pivottablerefreshoption/
---
## PivotTableRefreshOption constructor

Represents the options of refreshing data source of the pivot table.

```csharp
public PivotTableRefreshOption()
```

### Examples

```csharp
// Called: PivotTableRefreshOption option = new PivotTableRefreshOption();
[Test]
        public void PivotTableRefreshOption_Constructor()
        {
            Workbook wbk = new Workbook(Constants.PivotTableSourcePath + "CellsNet55242.xlsx");
            Worksheet wks = wbk.Worksheets[0];
            var cells = wks.Cells;

            cells.InsertRow(0);

            cells.InsertRows(5, 23, true);


            for (int count = 0, row = 5; count < 24; count++, row++)
            {
                var yearCell = cells[row, 1];
                var monthCell = cells[row, 2];
                var salesCell = cells[row, 3];

                yearCell.Value = (double)(2019 + count / 12);
                monthCell.Value = (double)(count % 12 + 1);
                salesCell.Value = 2000 + count * 1000.0 / 12;
            }
            PivotTableRefreshOption option = new PivotTableRefreshOption();
            option.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            wks.PivotTables[0].RefreshData(option);
            wks.PivotTables[0].CalculateData();
            wks.Charts[0].RefreshPivotData();
            wbk.Save(Constants.PivotTableDestPath + "CellsNet55242.xlsx", (SaveFormat)wbk.FileFormat);
            Assert.AreEqual(2, wks.PivotTables[0].RowFields[0].PivotItems.Count);

          
        }
```

### See Also

* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


