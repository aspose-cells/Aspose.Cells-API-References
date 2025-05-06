---
title: SqlScriptSaveOptions.IdName
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Gets and sets the name of id column
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/idname/
---
## SqlScriptSaveOptions.IdName property

Gets and sets the name of id column.

```csharp
public string IdName { get; set; }
```

### Remarks

If this property is set , a column will be inserted with automatical increment int value.

### Examples

```csharp
// Called: IdName = &amp;quot;ID&amp;quot;,
public static void Property_IdName()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill worksheet with some data
            worksheet.Cells[0, 0].PutValue(&quot;ID&quot;);
            worksheet.Cells[0, 1].PutValue(&quot;Name&quot;);
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue(&quot;John Doe&quot;);
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue(&quot;Jane Doe&quot;);

            // Create an instance of SqlScriptSaveOptions
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                ColumnTypeMap = new SqlScriptColumnTypeMap(),
                CheckAllDataForColumnType = true,
                AddBlankLineBetweenRows = false,
                Separator = &apos;;&apos;,
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = &quot;ID&quot;,
                StartId = 1,
                TableName = &quot;MyTable&quot;,
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ClearData = false,
                CachedFileFolder = &quot;C:\\Temp&quot;,
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                WarningCallback = null,
                UpdateSmartArt = false
            };

            // Save the workbook as SQL script
            workbook.Save(&quot;MyTable.sql&quot;, saveOptions);

            return;
        }
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


