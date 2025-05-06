---
title: PivotTable.DataSource
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the data source of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/datasource/
---
## PivotTable.DataSource property

Gets and sets the data source of the pivot table.

```csharp
public string[] DataSource { get; set; }
```

### Examples

```csharp
// Called: if (pivotTableColl[i].DataSource[j].IndexOf(rangeName, StringComparison.OrdinalIgnoreCase) != -1)
private static void Property_DataSource(Workbook workBook, string worksheetName, DataTable dataTable, int startingRow, int startingCol, bool isIncludeHeaders)
        {

            startingRow = startingRow != 0 ? startingRow - 1 : startingRow;
            startingCol = startingCol != 0 ? startingCol - 1 : startingCol;


            Worksheet ws = workBook.Worksheets[worksheetName];
            if (ws == null)
            {
                ws = workBook.Worksheets.Add(worksheetName);
            }
            else
            {
                //ws.Cells.Clear();
                int lastRow = ws.Cells.LastCell != null ? ws.Cells.LastCell.Row : 0;
                int lastCol = ws.Cells.LastCell != null ? ws.Cells.LastCell.Column : 0;

                lastRow = lastRow &gt; startingRow ? lastRow : startingRow;
                lastCol = lastCol &gt; startingCol ? lastCol : startingCol;

                ws.Cells.DeleteRange(startingRow, startingCol, lastRow, lastCol, ShiftType.None);
            }

            #region populate ws from dataTable
            int rowNumber = startingRow;
            if (isIncludeHeaders)
            {
                for (int i = 0; i &lt; dataTable.Columns.Count; i++)
                {

                    ws.Cells[startingRow, startingCol + i].PutValue(dataTable.Columns[i].ColumnName);
                    Style cellStyle = ws.Cells[startingRow, startingCol + i].GetStyle();
                    cellStyle.Font.IsBold = true;
                    ws.Cells[startingRow, startingCol + i].SetStyle(cellStyle);

                }
                rowNumber++;
            }

            int excelRowNo = rowNumber;
            int pageCount = 0;
            foreach (DataRow row in dataTable.Rows)
            {

                for (int i = 0; i &lt; dataTable.Columns.Count; i++)
                {
                    if (dataTable.Columns[i].DataType == typeof(DateTime))
                    {
                        ws.Cells[excelRowNo, startingCol + i].GetStyle().Number = 14;
                    }
                    else if (dataTable.Columns[i].DataType == typeof(decimal))
                    {
                        ws.Cells[excelRowNo, startingCol + i].GetStyle().Number = 2;
                    }

                    ws.Cells[excelRowNo, startingCol + i].PutValue(row.ItemArray[i]);
                }

                excelRowNo++;
                rowNumber++;
            }
            ws.AutoFitColumns();
            #endregion

            Aspose.Cells.Range[] allRanges = workBook.Worksheets.GetNamedRanges();

            //if xls template does not have any NamedRanges, it returns a null
            if (allRanges != null)
            {
                //spin thru NamedRanges and see if the parent ws is the ws that we just refreshed from the database
                string rangeName = null;
                foreach (Aspose.Cells.Range rangeItem in allRanges)
                {
                    if (string.Equals(rangeItem.Worksheet.Name, worksheetName, StringComparison.OrdinalIgnoreCase))
                    {
                        //first remove the old
                        rangeName = rangeItem.Name;
                        workBook.Worksheets.Names.Remove(rangeName);

                        //creates a new named range with the same name
                        Aspose.Cells.Range newRange = ws.Cells.CreateRange(startingRow, startingCol, dataTable.Rows.Count + 1, dataTable.Columns.Count);     //rows+1 needed to allow for header
                        newRange.Name = rangeName;
                        ws.AutoFitColumns(); // auto fit columns
                        break;
                    }

                }

                //refresh named Ranges
                allRanges = workBook.Worksheets.GetNamedRanges();

                if (String.IsNullOrEmpty(rangeName))
                {
                    throw new Exception(String.Format(&quot;An Error occurred while filling worksheet {0} because it does not contain any named range&quot;, worksheetName));
                }


                foreach (Worksheet itemWs in workBook.Worksheets)
                {
                    var pivotTableColl = itemWs.PivotTables;
                    for (int i = 0; i &lt; pivotTableColl.Count; i++)
                    {
                        for (int j = 0; j &lt; pivotTableColl[i].DataSource.Length; j++)
                        {
                            if (pivotTableColl[i].DataSource[j].IndexOf(rangeName, StringComparison.OrdinalIgnoreCase) != -1)
                            {
                                pivotTableColl[i].PreserveFormatting = true;
                                pivotTableColl[i].RefreshData();
                                pivotTableColl[i].CalculateData();
                            }
                        }
                    }
                }


                //sets the active sheet to 0
                workBook.Worksheets.ActiveSheetIndex = 0;
            }
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


