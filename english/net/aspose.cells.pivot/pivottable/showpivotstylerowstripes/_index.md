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
            string filePath = Constants.PivotTableSourcePath + @"NET43901_";
            DataTable data = new DataTable();
            data.Columns.Add(new DataColumn("Workspace_Id"));
            data.Columns.Add(new DataColumn("Entity_Id"));
            data.Columns.Add(new DataColumn("Vulnerability"));
            data.Columns.Add(new DataColumn("Year"));
            data.Columns.Add(new DataColumn("Number"));
            data.Columns.Add(new DataColumn("OS Version"));

            Random rand = new Random();

            for (int i = 0; i < 5; i++)
            {
                int randNumber = rand.Next(200, 1000);
                int randVersion = rand.Next(5, 20);
                int randWorkspace = rand.Next(28, 30);
                int randEntity = rand.Next(30, 40);

                DataRow row = data.NewRow();
                row["Workspace_Id"] = randWorkspace;
                row["Entity_Id"] = randEntity;
                row["Vulnerability"] = RandomString43901(50);//Path.GetRandomFileName().Replace(".", "").Substring(0, 8); ;
                row["Year"] = "2001";
                row["Number"] = randNumber;
                row["OS Version"] = randVersion;

                data.Rows.Add(row);
            }

            Workbook wb_a = new Workbook(filePath + "wbA.xlsx");
            Workbook wb_b = new Workbook(filePath + "wbB.xlsx");
            wb_a.Combine(wb_b);
            wb_a.Worksheets["SheetB"].Cells.ImportData(data, 7, 7, new ImportTableOptions()
            {
                IsFieldNameShown = false,
                InsertRows = false,
                ConvertNumericData = true,
                TotalRows = 5,
                TotalColumns = 6,
                DateFormat = "mm/dd/yy hh:mm AM/PM"
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
            wb_a.Save(Constants.PIVOT_CHECK_FILE_PATH + @"NET43901_SheetB_PiovtTable1_wrapText.xlsx");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


