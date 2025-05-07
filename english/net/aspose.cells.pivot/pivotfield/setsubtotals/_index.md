---
title: PivotField.SetSubtotals
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the specified field shows that subtotals
type: docs
url: /net/aspose.cells.pivot/pivotfield/setsubtotals/
---
## PivotField.SetSubtotals method

Sets whether the specified field shows that subtotals.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | subtotals type. |
| shown | Boolean | whether the specified field shows that subtotals. |

### Examples

```csharp
// Called: pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
[Test]
        public void Method_Boolean_()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET42168_";

            //Instantiating an Workbook object
            Workbook workbook = new Workbook();
            //Obtaining the reference of the first worksheet
            Worksheet sheet = workbook.Worksheets[0];
            //Name the sheet
            sheet.Name = "Data";
            Cells cells = sheet.Cells;

            #region Setting the values to the cells
            Cell cell = cells["A1"];
            cell.PutValue("Employee");
            cell = cells["B1"];
            cell.PutValue("Quarter");
            cell = cells["C1"];
            cell.PutValue("Product");
            //cell = cells["D1"];
            //cell.PutValue("Continent");
            //cell = cells["E1"];
            //cell.PutValue("Country");
            //cell = cells["F1"];
            //cell.PutValue("Sale");
            cell = cells["A2"];
            cell.PutValue("David");
            cell = cells["A3"];
            cell.PutValue("David");
            cell = cells["A4"];
            cell.PutValue("David");
            cell = cells["A5"];
            cell.PutValue("David");
            cell = cells["A6"];
            cell.PutValue("James");
            cell = cells["A7"];
            cell.PutValue("James");
            cell = cells["A8"];
            cell.PutValue("James");
            cell = cells["A9"];
            cell.PutValue("James");
            cell = cells["A10"];
            cell.PutValue("James");
            cell = cells["A11"];
            cell.PutValue("Miya");
            cell = cells["A12"];
            cell.PutValue("Miya");
            cell = cells["A13"];
            cell.PutValue("Miya");
            cell = cells["A14"];
            cell.PutValue("Miya");
            cell = cells["A15"];
            cell.PutValue("Miya");
            cell = cells["A16"];
            cell.PutValue("Miya");
            cell = cells["A17"];
            cell.PutValue("Miya");
            cell = cells["A18"];
            cell.PutValue("Elvis");
            cell = cells["A19"];
            cell.PutValue("Elvis");
            cell = cells["A20"];
            cell.PutValue("Elvis");
            cell = cells["A21"];
            cell.PutValue("Elvis");
            cell = cells["A22"];
            cell.PutValue("Elvis");
            cell = cells["A23"];
            cell.PutValue("Elvis");
            cell = cells["A24"];
            cell.PutValue("Elvis");
            cell = cells["A25"];
            cell.PutValue("Jean");
            cell = cells["A26"];
            cell.PutValue("Jean");
            cell = cells["A27"];
            cell.PutValue("Jean");
            cell = cells["A28"];
            cell.PutValue("Ada");
            cell = cells["A29"];
            cell.PutValue("Ada");
            cell = cells["A30"];
            cell.PutValue("Ada");

            cell = cells["B2"];
            cell.PutValue("1");
            cell = cells["B3"];
            cell.PutValue("2");
            cell = cells["B4"];
            cell.PutValue("3");
            cell = cells["B5"];
            cell.PutValue("4");
            cell = cells["B6"];
            cell.PutValue("1");
            cell = cells["B7"];
            cell.PutValue("2");
            cell = cells["B8"];
            cell.PutValue("3");
            cell = cells["B9"];
            cell.PutValue("4");
            cell = cells["B10"];
            cell.PutValue("4");
            cell = cells["B11"];
            cell.PutValue("1");
            cell = cells["B12"];
            cell.PutValue("1");
            cell = cells["B13"];
            cell.PutValue("2");
            cell = cells["B14"];
            cell.PutValue("2");
            cell = cells["B15"];
            cell.PutValue("3");
            cell = cells["B16"];
            cell.PutValue("4");
            cell = cells["B17"];
            cell.PutValue("4");
            cell = cells["B18"];
            cell.PutValue("1");
            cell = cells["B19"];
            cell.PutValue("1");
            cell = cells["B20"];
            cell.PutValue("2");
            cell = cells["B21"];
            cell.PutValue("3");
            cell = cells["B22"];
            cell.PutValue("3");
            cell = cells["B23"];
            cell.PutValue("4");
            cell = cells["B24"];
            cell.PutValue("4");
            cell = cells["B25"];
            cell.PutValue("1");
            cell = cells["B26"];
            cell.PutValue("2");
            cell = cells["B27"];
            cell.PutValue("3");
            cell = cells["B28"];
            cell.PutValue("1");
            cell = cells["B29"];
            cell.PutValue("2");
            cell = cells["B30"];
            cell.PutValue("3");

            cell = cells["C2"];
            cell.PutValue("Maxilaku");
            cell = cells["C3"];
            cell.PutValue("Maxilaku");
            cell = cells["C4"];
            cell.PutValue("Chai");
            cell = cells["C5"];
            cell.PutValue("Maxilaku");
            cell = cells["C6"];
            cell.PutValue("Chang");
            cell = cells["C7"];
            cell.PutValue("Chang");
            cell = cells["C8"];
            cell.PutValue("Chang");
            cell = cells["C9"];
            cell.PutValue("Chang");
            cell = cells["C10"];
            cell.PutValue("Chang");
            cell = cells["C11"];
            cell.PutValue("Geitost");
            cell = cells["C12"];
            cell.PutValue("Chai");
            cell = cells["C13"];
            cell.PutValue("Geitost");
            cell = cells["C14"];
            cell.PutValue("Geitost");
            cell = cells["C15"];
            cell.PutValue("Maxilaku");
            cell = cells["C16"];
            cell.PutValue("Geitost");
            cell = cells["C17"];
            cell.PutValue("Geitost");
            cell = cells["C18"];
            cell.PutValue("Ikuru");
            cell = cells["C19"];
            cell.PutValue("Ikuru");
            cell = cells["C20"];
            cell.PutValue("Ikuru");
            cell = cells["C21"];
            cell.PutValue("Ikuru");
            cell = cells["C22"];
            cell.PutValue("Ipoh Coffee");
            cell = cells["C23"];
            cell.PutValue("Ipoh Coffee");
            cell = cells["C24"];
            cell.PutValue("Ipoh Coffee");
            cell = cells["C25"];
            cell.PutValue("Chocolade");
            cell = cells["C26"];
            cell.PutValue("Chocolade");
            cell = cells["C27"];
            cell.PutValue("Chocolade");
            cell = cells["C28"];
            cell.PutValue("Chocolade");
            cell = cells["C29"];
            cell.PutValue("Chocolade");
            cell = cells["C30"];
            cell.PutValue("Chocolade");
            #endregion

            //Adding a new sheet
            Worksheet sheet2 = workbook.Worksheets[workbook.Worksheets.Add()];
            //Naming the sheet
            sheet2.Name = "PivotTable";
            #region create pivottable
            //Getting the pivottables collection in the sheet
            Aspose.Cells.Pivot.PivotTableCollection pivotTables = sheet2.PivotTables;
            //Adding a PivotTable to the worksheet
            int index = pivotTables.Add("=Data!A1:C30", "A1", "PivotTable1");
            //Accessing the instance of the newly added PivotTable
            Aspose.Cells.Pivot.PivotTable pivotTable = pivotTables[index];
            pivotTable.ShowRowGrandTotals = false;
            pivotTable.ShowColumnGrandTotals = false;
            pivotTable.IsAutoFormat = true;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Classic;

            int i = 0;
            int indexAddItem = 0;
            bool isSubTotal = false;
            bool isPagebreakView = false;

            for (i = 0; i < 3; i++)
            {
                isSubTotal = (i == 2 ? false : true);
                if (true)
                {
                    indexAddItem = pivotTable.AddFieldToArea(PivotFieldType.Row, i);
                    PivotField pivotField = pivotTable.RowFields[indexAddItem];

                    pivotField.IsAutoSort = true;
                    pivotField.IsAscendSort = true;
                    pivotField.AutoSortField = -1;

                    pivotField.IsAutoSubtotals = isSubTotal;

                    if (isSubTotal == true)
                    {
                        pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
                    }
                    if ((i == 2 ? false : true))
                    {
                        indexAddItem = pivotTable.AddFieldToArea(PivotFieldType.Data, i);

                        PivotField pivotFieldData = pivotTable.DataFields[indexAddItem];
                        pivotFieldData.Function = ConsolidationFunction.Sum;
                    }
                }
            }
            #endregion
            sheet2.IsPageBreakPreview = isPagebreakView;

            //Saving the Excel file            
            MemoryStream stream = workbook.SaveToStream();
            //workbook.Save(CreateFolder(filePath) + "out.xlsx");
        }
```

### See Also

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


