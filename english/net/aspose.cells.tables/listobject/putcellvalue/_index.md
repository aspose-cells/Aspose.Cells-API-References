---
title: ListObject.PutCellValue
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Put the value to the cell
type: docs
url: /net/aspose.cells.tables/listobject/putcellvalue/
---
## PutCellValue(int, int, object) {#putcellvalue}

Put the value to the cell.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| value | Object | The cell value. |

### Examples

```csharp
// Called: listObjects[1].PutCellValue(3, 0, 3);
[Test]
        public void Method_Object_()
        {
            Workbook workbook = new Workbook();

            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // Test formula outside of Table ================================================
            // Adding values to cells
            worksheet.Cells.SetColumnWidth(0, 20);
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Outside table&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(1);
            worksheet.Cells[&quot;A4&quot;].PutValue(2);
            worksheet.Cells[&quot;A5&quot;].PutValue(3);
            // Adding a formula
            worksheet.Cells[&quot;A6&quot;].Formula = &quot;=SUM(A1:A3)&quot;;
            worksheet.Cells[&quot;A7&quot;].Formula = &quot;=SUM(C1:C3)&quot;;

            // Test cell.formula inside of Table ============================================
            worksheet.Cells.SetColumnWidth(2, 20);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Inside table: cell.formula&quot;);

            Aspose.Cells.Tables.ListObjectCollection listObjects = worksheet.ListObjects;
            listObjects.Add(&quot;C2&quot;, &quot;C7&quot;, true);

            worksheet.Cells[&quot;C3&quot;].PutValue(1);
            worksheet.Cells[&quot;C4&quot;].PutValue(2);
            worksheet.Cells[&quot;C5&quot;].PutValue(3);

            // Adding a formula trought cell.value
            worksheet.Cells[&quot;C6&quot;].Formula = &quot;=SUM(C1:C3)&quot;;
            worksheet.Cells[&quot;C7&quot;].Formula = &quot;=SUM(A1:A3)&quot;;



            // Test listObjects.PutCellValue inside of Table ================================
            worksheet.Cells.SetColumnWidth(4, 20);
            worksheet.Cells[&quot;E1&quot;].PutValue(&quot;Inside table: listObjects.PutCellValue&quot;);

            listObjects.Add(&quot;E2&quot;, &quot;E7&quot;, true);

            listObjects[1].PutCellValue(1, 0, 1);
            listObjects[1].PutCellValue(2, 0, 2);
            listObjects[1].PutCellValue(3, 0, 3);

            // Adding a formula trought listObjects.PutCellValue
            listObjects[1].PutCellFormula(4, 0, &quot;=SUM(C1:C3)&quot;);
            listObjects[1].PutCellFormula(5, 0, &quot;=SUM(A1:A3)&quot;);
            Assert.AreEqual(&quot;=SUM(A1:A3)&quot;, worksheet.Cells[&quot;E7&quot;].Formula);

            // Calculating the results of formulas
            workbook.CalculateFormula();

            workbook.Save(Constants.destPath + &quot;CELLSNET53064.xlsx&quot;);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellValue(int, int, object, bool) {#putcellvalue_1}

Put the value to the cell.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value, bool isTotalsRowLabel)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| value | Object | The cell value. |
| isTotalsRowLabel | Boolean | Indicates whether it is a label for total row,only works for total row. If False and this row is total row, a new row will be inserted. |

### Examples

```csharp
// Called: listObject.PutCellValue(3, colOffset, 33.333, false);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET53325.xlsx&quot;);
            ListObjectCollection listObjects = workbook.Worksheets[0].ListObjects;
            for (int sheetIndex = 0; sheetIndex &lt; workbook.Worksheets.Count; sheetIndex++)
            {
                foreach (ListObject listObject in workbook.Worksheets[sheetIndex].ListObjects)
                {
                    int tableWidth = listObject.EndColumn - listObject.StartColumn;

                    for (int colOffset = 0; colOffset &lt;= tableWidth; colOffset++)
                    {
                        // Bug 2:
                        if (listObject.DisplayName.StartsWith(&quot;totalsTest&quot;))
                            listObject.ShowTotals = false;
                        // End Bug 2

                        if (listObject.DisplayName.StartsWith(&quot;Formatted&quot;))
                        { // Bug 3: write value as string to a table
                            listObject.PutCellValue(1, colOffset, &quot;11&quot;, false);
                            listObject.PutCellValue(2, colOffset, &quot;22&quot;, false);
                            listObject.PutCellValue(3, colOffset, &quot;33.333&quot;, false);

                        } // Bug 3 End

                        else
                        {
                            listObject.PutCellValue(1, colOffset, 11, false);
                            listObject.PutCellValue(2, colOffset, 22, false);
                            listObject.PutCellValue(3, colOffset, 33.333, false);

                        }
                        //Bug2:
                        if (listObject.DisplayName.StartsWith(&quot;totalsTest&quot;))
                            listObject.ShowTotals = true;
                        //    End Bug 2:
                    }
                }
            }

            // Good 3 : Write strings to formatted cells
            workbook.Worksheets[0].Cells[&quot;K10&quot;].PutValue(&quot;11&quot;, true);
            workbook.Worksheets[0].Cells[&quot;L11&quot;].PutValue(&quot;11,135&quot;, true);
            workbook.Worksheets[0].Cells[&quot;K10&quot;].PutValue(&quot;05.05.2023&quot;, true);
            workbook.Worksheets[0].Cells[&quot;L11&quot;].PutValue(&quot;05.05.2023&quot;, true);
            workbook.Settings.FormulaSettings.CalculateOnOpen = true;

            Style style = workbook.Worksheets[0].Cells[&quot;C25&quot;].GetDisplayStyle();
            Assert.IsTrue(Util.CompareColor( Color.FromArgb(91,155,213),style.ForegroundColor));
            Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + &quot;CELLSNET53325.xlsx&quot;);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


