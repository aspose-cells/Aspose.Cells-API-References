---
title: PivotTable.AutoFormatType
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the auto format type of PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/autoformattype/
---
## PivotTable.AutoFormatType property

Gets and sets the auto format type of PivotTable.

```csharp
public PivotTableAutoFormatType AutoFormatType { get; set; }
```

### Examples

```csharp
// Called: pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
[Test]
        public void Property_AutoFormatType()
        {
            Aspose.Cells.License license = new Aspose.Cells.License();
            license.SetLicense(Constants.licPath);

            var workbook = new Workbook();
            //Obtaining the reference of the first worksheet
            var sheet = workbook.Worksheets[0];
            //Name the sheet
            sheet.Name = "data";
            var cells = sheet.Cells;
            int urange = 1;

            cells["A" + urange].PutValue("State");
            cells["B" + urange].PutValue("City");
            cells["C" + urange].PutValue("Population");

            urange++;
            cells["A" + urange].PutValue("TN");
            cells["B" + urange].PutValue("Chennai");
            cells["C" + urange].PutValue("50");

            urange++;
            cells["A" + urange].PutValue("KL");
            cells["B" + urange].PutValue("Cochin");
            cells["C" + urange].PutValue("70");

            urange++;
            cells["A" + urange].PutValue("KA");
            cells["B" + urange].PutValue("Bangalore");
            cells["C" + urange].PutValue("80");

            urange++;
            cells["A" + urange].PutValue("AP");
            cells["B" + urange].PutValue("Hydrapad");
            cells["C" + urange].PutValue("63");

            var listObject = sheet.ListObjects[sheet.ListObjects.Add("A1", "C5", true)];

            //To fit the column as per test size.
            sheet.AutoFitColumns(0, 26);

            //Adding Default Style to the table

            listObject.TableStyleType = TableStyleType.None;

            var sheet2 = workbook.Worksheets[workbook.Worksheets.Add()];

            //Naming the sheet
            sheet2.Name = "PivotSheet";

            //Getting the pivottables collection in the sheet
            var pivotTables = sheet2.PivotTables;
            //Adding a PivotTable to the worksheet
            var index = pivotTables.Add("=" + sheet.Name + "!A1:C5", "A1", sheet2.Name);

            //To fit the column as per test size.
            sheet2.AutoFitColumns(0, 24);

            //Accessing the instance of the newly added PivotTable
            PivotTable pivotTable = pivotTables[index];

            //Showing the grand totals
            pivotTable.ShowRowGrandTotals = false;
            pivotTable.ShowColumnGrandTotals = false;
            pivotTable.IsAutoFormat = true;

            pivotTable.RowHeaderCaption = "State";
            pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
            pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight1;

            pivotTable.AddFieldToArea(PivotFieldType.Row, "State");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "City");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Population");

            var pivotFields = pivotTable.RowFields;

            //Hide the subtotal.
            for (var i = 0; i < pivotFields.Count; i++)
            {
                pivotTable.RowFields[i].SetSubtotals(PivotFieldSubtotalType.None, true);
            }
            sheet2.MoveTo(0);//Move PivotTable Sheets to 0th Position in the workbook

            //for auto-testing
            int activeIndex = -1;
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                if (workbook.Worksheets[i].IsSelected)
                {
                    activeIndex = i;
                    break;
                }
            }
            Assert.AreNotEqual(activeIndex, -1);
            Assert.AreEqual(workbook.Worksheets.ActiveSheetIndex, activeIndex);
            //end

            workbook.Save(Constants.PivotTableDestPath + @"NET43070.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* enum [PivotTableAutoFormatType](../../pivottableautoformattype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


