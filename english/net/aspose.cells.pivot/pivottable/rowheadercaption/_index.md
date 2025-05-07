---
title: PivotTable.RowHeaderCaption
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the Row Header Caption of the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/rowheadercaption/
---
## PivotTable.RowHeaderCaption property

Gets the Row Header Caption of the PivotTable.

```csharp
public string RowHeaderCaption { get; set; }
```

### Examples

```csharp
// Called: pivotTable.RowHeaderCaption = "ID";
[Test]
        public void Property_RowHeaderCaption()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CellsNet55115.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            int maxdatacol = worksheet.Cells.MaxDataColumn;
            int maxdatarow = worksheet.Cells.MaxDataRow;
            string cellname = CellsHelper.CellIndexToName(maxdatarow, maxdatacol);

            Worksheet pivotSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            Column column = pivotSheet.Cells.Columns[1];
            //Style style = column.GetStyle();
            //style.Number = 14;
            //column.SetStyle(style);

            PivotTable pivotTable = pivotSheet.PivotTables[pivotSheet.PivotTables.Add("=" + worksheet.Name + "!A1:" + cellname, "A1", "PivotTable1")];

            pivotTable.ShowRowGrandTotals = false;
            pivotTable.ShowColumnGrandTotals = false;
            pivotTable.ShowDrill = false;

            pivotTable.RowHeaderCaption = "ID";
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ID");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date Created");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Type");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "PayAmount");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "PivotColumn");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                pivotTable.RowFields[i].SetSubtotals(PivotFieldSubtotalType.None, true);
                pivotTable.RowFields[i].IsRepeatItemLabels = true;
            }
          

            pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Worksheet copySheet = workbook.Worksheets[workbook.Worksheets.Add()];

            copySheet.Cells.CopyRows(pivotSheet.Cells, 1, 0, pivotSheet.Cells.MaxDataRow);

            Assert.AreEqual("12/17/2023", copySheet.Cells["B4"].StringValue);

            workbook.Save(Constants.PivotTableDestPath + "CellsNet55115.xlsx");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


