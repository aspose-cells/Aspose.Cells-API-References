---
title: SqlScriptSaveOptions.ExportArea
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Gets or sets the exporting range
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/exportarea/
---
## SqlScriptSaveOptions.ExportArea property

Gets or sets the exporting range.

```csharp
public CellArea ExportArea { get; set; }
```

### Examples

```csharp
// Called: ExportArea = new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 1 },
public static void Property_ExportArea()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;ID&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(1);
            worksheet.Cells[&quot;A3&quot;].PutValue(2);
            worksheet.Cells[&quot;A4&quot;].PutValue(3);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Name&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(&quot;Alice&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(&quot;Bob&quot;);
            worksheet.Cells[&quot;B4&quot;].PutValue(&quot;Charlie&quot;);

            // Create SqlScriptSaveOptions and set properties
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                AddBlankLineBetweenRows = true,
                Separator = &apos;;&apos;,
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = &quot;ID&quot;,
                StartId = 1,
                TableName = &quot;SampleTable&quot;,
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Save the workbook as SQL script
            workbook.Save(&quot;SqlScriptOperatorTypeExample.sql&quot;, saveOptions);

            // Output the results
            Console.WriteLine(&quot;SQL script has been saved successfully.&quot;);
        }
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


