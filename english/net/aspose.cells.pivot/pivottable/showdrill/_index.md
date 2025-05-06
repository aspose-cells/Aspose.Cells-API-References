---
title: PivotTable.ShowDrill
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets whether showing expand/collapse buttons
type: docs
url: /net/aspose.cells.pivot/pivottable/showdrill/
---
## PivotTable.ShowDrill property

Gets and sets whether showing expand/collapse buttons.

```csharp
public bool ShowDrill { get; set; }
```

### Examples

```csharp
// Called: xlsPivotTable.ShowDrill = false;
[Test]
        public void Property_ShowDrill()
        {
            Workbook xlsWorkbook = new Workbook(Constants.openPivottablePath + &quot;SalesRpt.xlsx&quot;);
            Worksheet xlsWorksheet = xlsWorkbook.Worksheets[&quot;Sheet2&quot;];
            xlsWorkbook.Worksheets.Names.Remove(&quot;Raw_Data&quot;);
            xlsWorksheet.Cells.DeleteRows(4, 4);
            Cells cells = xlsWorksheet.Cells;
            Cell cell = cells[&quot;A5&quot;];
            cell.PutValue(&quot;Golf&quot;);
            cell = cells[&quot;A6&quot;];
            cell.PutValue(&quot;Golf&quot;);
            cell = cells[&quot;A7&quot;];
            cell.PutValue(&quot;Outdoors&quot;);
            cell = cells[&quot;A8&quot;];
            cell.PutValue(&quot;Outdoors&quot;);
            cell = cells[&quot;A9&quot;];
            cell.PutValue(&quot;Outdoors&quot;);
            cell = cells[&quot;B5&quot;];
            cell.PutValue(&quot;Golf Balls&quot;);
            cell = cells[&quot;B6&quot;];
            cell.PutValue(&quot;Clubs&quot;);
            cell = cells[&quot;B7&quot;];
            cell.PutValue(&quot;Tents&quot;);
            cell = cells[&quot;B8&quot;];
            cell.PutValue(&quot;Fishing Poles&quot;);
            cell = cells[&quot;B9&quot;];
            cell.PutValue(&quot;Bug Spray&quot;);
            cell = cells[&quot;C5&quot;];
            cell.PutValue(25);
            cell = cells[&quot;C6&quot;];
            cell.PutValue(21);
            cell = cells[&quot;C7&quot;];
            cell.PutValue(42);
            cell = cells[&quot;C8&quot;];
            cell.PutValue(58);
            cell = cells[&quot;C9&quot;];
            cell.PutValue(74);
            cell = cells[&quot;D5&quot;];
            cell.PutValue(34);
            cell = cells[&quot;D6&quot;];
            cell.PutValue(14);
            cell = cells[&quot;D7&quot;];
            cell.PutValue(62);
            cell = cells[&quot;D8&quot;];
            cell.PutValue(71);
            cell = cells[&quot;D9&quot;];
            cell.PutValue(36);
            Aspose.Cells.Range rgeDtaSource = xlsWorksheet.Cells.CreateRange(3, 0, 6, 4);
            rgeDtaSource.Name = &quot;Raw_Data&quot;;
            foreach (Worksheet ws in xlsWorkbook.Worksheets)
            {
                foreach (PivotTable xlsPivotTable in ws.PivotTables)
                {
                    xlsPivotTable.IsAutoFormat = false;
                    xlsPivotTable.ShowDrill = false;

                    xlsPivotTable.RefreshData();
                    //xlsPivotTable.RefreshDataOnOpeningFile = true;
                    xlsPivotTable.CalculateData();

                }
            }
            xlsWorkbook.Save(Constants.savePivottablePath + &quot;29876.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


