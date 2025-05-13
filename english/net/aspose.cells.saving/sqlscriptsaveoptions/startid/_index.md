---
title: SqlScriptSaveOptions.StartId
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Gets and sets the start id
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/startid/
---
## SqlScriptSaveOptions.StartId property

Gets and sets the start id.

```csharp
public int StartId { get; set; }
```

### Remarks

Only works when [`IdName`](../idname/) is set.

### Examples

```csharp
// Called: StartId = 1,
public static void SqlScriptSaveOptions_Property_StartId()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill worksheet with some data
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Name");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue("John Doe");
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("Jane Doe");

            // Create an instance of SqlScriptSaveOptions
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                ColumnTypeMap = new SqlScriptColumnTypeMap(),
                CheckAllDataForColumnType = true,
                AddBlankLineBetweenRows = false,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "MyTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                WarningCallback = null,
                UpdateSmartArt = false
            };

            // Save the workbook as SQL script
            workbook.Save("MyTable.sql", saveOptions);

            return;
        }
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


