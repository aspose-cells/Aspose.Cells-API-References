---
title: PivotTable.ShowRowGrandTotals
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether to show grand totals for rows of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/showrowgrandtotals/
---
## PivotTable.ShowRowGrandTotals property

Indicates whether to show grand totals for rows of the pivot table.

```csharp
public bool ShowRowGrandTotals { get; set; }
```

### Examples

```csharp
// Called: pivotTable.ShowRowGrandTotals = false;
[Test]
        public void Property_ShowRowGrandTotals()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET42168_&quot;;

            //Instantiating an Workbook object
            Workbook workbook = new Workbook();
            //Obtaining the reference of the first worksheet
            Worksheet sheet = workbook.Worksheets[0];
            //Name the sheet
            sheet.Name = &quot;Data&quot;;
            Cells cells = sheet.Cells;

            #region Setting the values to the cells
            Cell cell = cells[&quot;A1&quot;];
            cell.PutValue(&quot;Employee&quot;);
            cell = cells[&quot;B1&quot;];
            cell.PutValue(&quot;Quarter&quot;);
            cell = cells[&quot;C1&quot;];
            cell.PutValue(&quot;Product&quot;);
            //cell = cells[&quot;D1&quot;];
            //cell.PutValue(&quot;Continent&quot;);
            //cell = cells[&quot;E1&quot;];
            //cell.PutValue(&quot;Country&quot;);
            //cell = cells[&quot;F1&quot;];
            //cell.PutValue(&quot;Sale&quot;);
            cell = cells[&quot;A2&quot;];
            cell.PutValue(&quot;David&quot;);
            cell = cells[&quot;A3&quot;];
            cell.PutValue(&quot;David&quot;);
            cell = cells[&quot;A4&quot;];
            cell.PutValue(&quot;David&quot;);
            cell = cells[&quot;A5&quot;];
            cell.PutValue(&quot;David&quot;);
            cell = cells[&quot;A6&quot;];
            cell.PutValue(&quot;James&quot;);
            cell = cells[&quot;A7&quot;];
            cell.PutValue(&quot;James&quot;);
            cell = cells[&quot;A8&quot;];
            cell.PutValue(&quot;James&quot;);
            cell = cells[&quot;A9&quot;];
            cell.PutValue(&quot;James&quot;);
            cell = cells[&quot;A10&quot;];
            cell.PutValue(&quot;James&quot;);
            cell = cells[&quot;A11&quot;];
            cell.PutValue(&quot;Miya&quot;);
            cell = cells[&quot;A12&quot;];
            cell.PutValue(&quot;Miya&quot;);
            cell = cells[&quot;A13&quot;];
            cell.PutValue(&quot;Miya&quot;);
            cell = cells[&quot;A14&quot;];
            cell.PutValue(&quot;Miya&quot;);
            cell = cells[&quot;A15&quot;];
            cell.PutValue(&quot;Miya&quot;);
            cell = cells[&quot;A16&quot;];
            cell.PutValue(&quot;Miya&quot;);
            cell = cells[&quot;A17&quot;];
            cell.PutValue(&quot;Miya&quot;);
            cell = cells[&quot;A18&quot;];
            cell.PutValue(&quot;Elvis&quot;);
            cell = cells[&quot;A19&quot;];
            cell.PutValue(&quot;Elvis&quot;);
            cell = cells[&quot;A20&quot;];
            cell.PutValue(&quot;Elvis&quot;);
            cell = cells[&quot;A21&quot;];
            cell.PutValue(&quot;Elvis&quot;);
            cell = cells[&quot;A22&quot;];
            cell.PutValue(&quot;Elvis&quot;);
            cell = cells[&quot;A23&quot;];
            cell.PutValue(&quot;Elvis&quot;);
            cell = cells[&quot;A24&quot;];
            cell.PutValue(&quot;Elvis&quot;);
            cell = cells[&quot;A25&quot;];
            cell.PutValue(&quot;Jean&quot;);
            cell = cells[&quot;A26&quot;];
            cell.PutValue(&quot;Jean&quot;);
            cell = cells[&quot;A27&quot;];
            cell.PutValue(&quot;Jean&quot;);
            cell = cells[&quot;A28&quot;];
            cell.PutValue(&quot;Ada&quot;);
            cell = cells[&quot;A29&quot;];
            cell.PutValue(&quot;Ada&quot;);
            cell = cells[&quot;A30&quot;];
            cell.PutValue(&quot;Ada&quot;);

            cell = cells[&quot;B2&quot;];
            cell.PutValue(&quot;1&quot;);
            cell = cells[&quot;B3&quot;];
            cell.PutValue(&quot;2&quot;);
            cell = cells[&quot;B4&quot;];
            cell.PutValue(&quot;3&quot;);
            cell = cells[&quot;B5&quot;];
            cell.PutValue(&quot;4&quot;);
            cell = cells[&quot;B6&quot;];
            cell.PutValue(&quot;1&quot;);
            cell = cells[&quot;B7&quot;];
            cell.PutValue(&quot;2&quot;);
            cell = cells[&quot;B8&quot;];
            cell.PutValue(&quot;3&quot;);
            cell = cells[&quot;B9&quot;];
            cell.PutValue(&quot;4&quot;);
            cell = cells[&quot;B10&quot;];
            cell.PutValue(&quot;4&quot;);
            cell = cells[&quot;B11&quot;];
            cell.PutValue(&quot;1&quot;);
            cell = cells[&quot;B12&quot;];
            cell.PutValue(&quot;1&quot;);
            cell = cells[&quot;B13&quot;];
            cell.PutValue(&quot;2&quot;);
            cell = cells[&quot;B14&quot;];
            cell.PutValue(&quot;2&quot;);
            cell = cells[&quot;B15&quot;];
            cell.PutValue(&quot;3&quot;);
            cell = cells[&quot;B16&quot;];
            cell.PutValue(&quot;4&quot;);
            cell = cells[&quot;B17&quot;];
            cell.PutValue(&quot;4&quot;);
            cell = cells[&quot;B18&quot;];
            cell.PutValue(&quot;1&quot;);
            cell = cells[&quot;B19&quot;];
            cell.PutValue(&quot;1&quot;);
            cell = cells[&quot;B20&quot;];
            cell.PutValue(&quot;2&quot;);
            cell = cells[&quot;B21&quot;];
            cell.PutValue(&quot;3&quot;);
            cell = cells[&quot;B22&quot;];
            cell.PutValue(&quot;3&quot;);
            cell = cells[&quot;B23&quot;];
            cell.PutValue(&quot;4&quot;);
            cell = cells[&quot;B24&quot;];
            cell.PutValue(&quot;4&quot;);
            cell = cells[&quot;B25&quot;];
            cell.PutValue(&quot;1&quot;);
            cell = cells[&quot;B26&quot;];
            cell.PutValue(&quot;2&quot;);
            cell = cells[&quot;B27&quot;];
            cell.PutValue(&quot;3&quot;);
            cell = cells[&quot;B28&quot;];
            cell.PutValue(&quot;1&quot;);
            cell = cells[&quot;B29&quot;];
            cell.PutValue(&quot;2&quot;);
            cell = cells[&quot;B30&quot;];
            cell.PutValue(&quot;3&quot;);

            cell = cells[&quot;C2&quot;];
            cell.PutValue(&quot;Maxilaku&quot;);
            cell = cells[&quot;C3&quot;];
            cell.PutValue(&quot;Maxilaku&quot;);
            cell = cells[&quot;C4&quot;];
            cell.PutValue(&quot;Chai&quot;);
            cell = cells[&quot;C5&quot;];
            cell.PutValue(&quot;Maxilaku&quot;);
            cell = cells[&quot;C6&quot;];
            cell.PutValue(&quot;Chang&quot;);
            cell = cells[&quot;C7&quot;];
            cell.PutValue(&quot;Chang&quot;);
            cell = cells[&quot;C8&quot;];
            cell.PutValue(&quot;Chang&quot;);
            cell = cells[&quot;C9&quot;];
            cell.PutValue(&quot;Chang&quot;);
            cell = cells[&quot;C10&quot;];
            cell.PutValue(&quot;Chang&quot;);
            cell = cells[&quot;C11&quot;];
            cell.PutValue(&quot;Geitost&quot;);
            cell = cells[&quot;C12&quot;];
            cell.PutValue(&quot;Chai&quot;);
            cell = cells[&quot;C13&quot;];
            cell.PutValue(&quot;Geitost&quot;);
            cell = cells[&quot;C14&quot;];
            cell.PutValue(&quot;Geitost&quot;);
            cell = cells[&quot;C15&quot;];
            cell.PutValue(&quot;Maxilaku&quot;);
            cell = cells[&quot;C16&quot;];
            cell.PutValue(&quot;Geitost&quot;);
            cell = cells[&quot;C17&quot;];
            cell.PutValue(&quot;Geitost&quot;);
            cell = cells[&quot;C18&quot;];
            cell.PutValue(&quot;Ikuru&quot;);
            cell = cells[&quot;C19&quot;];
            cell.PutValue(&quot;Ikuru&quot;);
            cell = cells[&quot;C20&quot;];
            cell.PutValue(&quot;Ikuru&quot;);
            cell = cells[&quot;C21&quot;];
            cell.PutValue(&quot;Ikuru&quot;);
            cell = cells[&quot;C22&quot;];
            cell.PutValue(&quot;Ipoh Coffee&quot;);
            cell = cells[&quot;C23&quot;];
            cell.PutValue(&quot;Ipoh Coffee&quot;);
            cell = cells[&quot;C24&quot;];
            cell.PutValue(&quot;Ipoh Coffee&quot;);
            cell = cells[&quot;C25&quot;];
            cell.PutValue(&quot;Chocolade&quot;);
            cell = cells[&quot;C26&quot;];
            cell.PutValue(&quot;Chocolade&quot;);
            cell = cells[&quot;C27&quot;];
            cell.PutValue(&quot;Chocolade&quot;);
            cell = cells[&quot;C28&quot;];
            cell.PutValue(&quot;Chocolade&quot;);
            cell = cells[&quot;C29&quot;];
            cell.PutValue(&quot;Chocolade&quot;);
            cell = cells[&quot;C30&quot;];
            cell.PutValue(&quot;Chocolade&quot;);
            #endregion

            //Adding a new sheet
            Worksheet sheet2 = workbook.Worksheets[workbook.Worksheets.Add()];
            //Naming the sheet
            sheet2.Name = &quot;PivotTable&quot;;
            #region create pivottable
            //Getting the pivottables collection in the sheet
            Aspose.Cells.Pivot.PivotTableCollection pivotTables = sheet2.PivotTables;
            //Adding a PivotTable to the worksheet
            int index = pivotTables.Add(&quot;=Data!A1:C30&quot;, &quot;A1&quot;, &quot;PivotTable1&quot;);
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

            for (i = 0; i &lt; 3; i++)
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
            //workbook.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


