---
title: Cells.MaxDataRow
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum row index of cell which contains data
type: docs
url: /net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Maximum row index of cell which contains data.

```csharp
public int MaxDataRow { get; }
```

### Remarks

Return -1 if there is no cell which contains data.

### Examples

```csharp
// Called: dumpLastRow = maxRowTemplateFileSheet.Cells.MaxDataRow;
private void Property_MaxDataRow(Workbook tempWorkbook, ArrayList dumpSheetList)
        {
            int sheetNo = tempWorkbook.Worksheets.Count;
            ArrayList checkList = new ArrayList();

            for (int i = 0; i &lt; sheetNo; i++)
            {
                Worksheet sheet = tempWorkbook.Worksheets[i];
                PivotTableCollection tables = sheet.PivotTables;

                for (int j = 0; j &lt; tables.Count; j++)
                {

                    PivotTable table = tables[j];
                    String[] dsource = table.DataSource;

                    for (int s = 0; s &lt; dsource.Length; s++)
                    {
                        // loop on each pivot source data
                        String sheetName = dsource[s].Substring(0, dsource[s].IndexOf(&quot;!&quot;));
                        sheetName = sheetName.Replace(&quot;[{}=&apos;&apos;]+&quot;, &quot;&quot;);
                        Worksheet masterSheet = tempWorkbook.Worksheets[sheetName]; // master_data sheet is the source data of pivot table
                        int masterLastRow = masterSheet.Cells.MaxDataRow; // master_data sheet last row no
                        int dumpLastRow = masterLastRow; // considering base_data sheet and master_data sheet has same data rows

                        if (!checkList.Contains(sheetName))
                        { // check if pivot source sheet is already executed

                            String dumpSheetName = (string)dumpSheetList[0];
                            Worksheet maxRowTemplateFileSheet = tempWorkbook.Worksheets[dumpSheetName];

                            if (dumpSheetList.Contains(dumpSheetName))
                            {

                                masterSheet.Cells.DeleteBlankColumns();
                                masterSheet.Cells.DeleteBlankRows();
                                dumpLastRow = maxRowTemplateFileSheet.Cells.MaxDataRow;

                                if (masterLastRow &gt; dumpLastRow)
                                { // deleting the rows in master_data sheet if master_data sheet has lesser rows than base_data sheet
                                    int totalrows = masterLastRow - dumpLastRow;
                                    masterSheet.Cells.DeleteRows(dumpLastRow + 1, totalrows, true);

                                }
                                else if (dumpLastRow &gt; masterLastRow)
                                { // extend formulaes by copying the range in master_data sheet if master_data sheet has larger rows than base_data sheet

                                    Cells cells = masterSheet.Cells;
                                    int totalrows = dumpLastRow - masterLastRow;
                                    int columns = cells.Rows[0].LastDataCell.Column + 1;
                                    int firstrow = cells.MaxDataRow;
                                    int firstcol = cells.Rows[0].FirstDataCell.Column;

                                    Aspose.Cells.Range r3 = cells.CreateRange(firstrow, firstcol, 1, columns);
                                    Aspose.Cells.Range r4 = cells.CreateRange((firstrow + 1), firstcol, totalrows, columns);

                                    r4.CopyData(r3);
                                }
                                checkList.Add(sheetName);
                            }
                        }
                        dsource[s] = masterSheet.Cells.MaxDisplayRange.RefersTo;
                    }
                    table.DataSource = dsource; // update pivot source data range
                    table.RefreshData();
                    table.CalculateData();
                }
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


