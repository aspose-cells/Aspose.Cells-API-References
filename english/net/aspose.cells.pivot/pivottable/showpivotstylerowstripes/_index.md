---
title: PivotTable.ShowPivotStyleRowStripes
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether row stripe formatting is applied
type: docs
url: /net/aspose.cells.pivot/pivottable/showpivotstylerowstripes/
---
## PivotTable.ShowPivotStyleRowStripes property

Indicates whether row stripe formatting is applied.

```csharp
public bool ShowPivotStyleRowStripes { get; set; }
```

### Examples

```csharp
// Called: ptable.ShowPivotStyleRowStripes = true;
[Test]
        public void Property_ShowPivotStyleRowStripes()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET43901_&quot;;
            DataTable data = new DataTable();
            data.Columns.Add(new DataColumn(&quot;Workspace_Id&quot;));
            data.Columns.Add(new DataColumn(&quot;Entity_Id&quot;));
            data.Columns.Add(new DataColumn(&quot;Vulnerability&quot;));
            data.Columns.Add(new DataColumn(&quot;Year&quot;));
            data.Columns.Add(new DataColumn(&quot;Number&quot;));
            data.Columns.Add(new DataColumn(&quot;OS Version&quot;));

            Random rand = new Random();

            for (int i = 0; i &lt; 5; i++)
            {
                int randNumber = rand.Next(200, 1000);
                int randVersion = rand.Next(5, 20);
                int randWorkspace = rand.Next(28, 30);
                int randEntity = rand.Next(30, 40);

                DataRow row = data.NewRow();
                row[&quot;Workspace_Id&quot;] = randWorkspace;
                row[&quot;Entity_Id&quot;] = randEntity;
                row[&quot;Vulnerability&quot;] = RandomString43901(50);//Path.GetRandomFileName().Replace(&quot;.&quot;, &quot;&quot;).Substring(0, 8); ;
                row[&quot;Year&quot;] = &quot;2001&quot;;
                row[&quot;Number&quot;] = randNumber;
                row[&quot;OS Version&quot;] = randVersion;

                data.Rows.Add(row);
            }

            Workbook wb_a = new Workbook(filePath + &quot;wbA.xlsx&quot;);
            Workbook wb_b = new Workbook(filePath + &quot;wbB.xlsx&quot;);
            wb_a.Combine(wb_b);
            wb_a.Worksheets[&quot;SheetB&quot;].Cells.ImportData(data, 7, 7, new ImportTableOptions()
            {
                IsFieldNameShown = false,
                InsertRows = false,
                ConvertNumericData = true,
                TotalRows = 5,
                TotalColumns = 6,
                DateFormat = &quot;mm/dd/yy hh:mm AM/PM&quot;
            });

            foreach (Worksheet sheet in wb_a.Worksheets)
            {
                foreach (PivotTable ptable in sheet.PivotTables)
                {
                    ptable.ShowPivotStyleRowHeader = false;
                    ptable.ShowPivotStyleRowStripes = true;
                    ptable.RefreshDataOnOpeningFile = true;
                    ptable.RefreshData();
                }
                sheet.AutoFitRows();
            }
            wb_a.Save(Constants.PIVOT_CHECK_FILE_PATH + @&quot;NET43901_SheetB_PiovtTable1_wrapText.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


