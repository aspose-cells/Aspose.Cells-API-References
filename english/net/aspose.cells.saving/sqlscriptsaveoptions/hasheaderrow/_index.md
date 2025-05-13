---
title: SqlScriptSaveOptions.HasHeaderRow
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Indicates whether the range contains header row
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/
---
## SqlScriptSaveOptions.HasHeaderRow property

Indicates whether the range contains header row.

```csharp
public bool HasHeaderRow { get; set; }
```

### Examples

```csharp
// Called: HasHeaderRow = true
public static void SqlScriptSaveOptions_Property_HasHeaderRow()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Create SqlScriptSaveOptions and set properties
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                AddBlankLineBetweenRows = true,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "SampleTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Save the workbook as SQL script
            workbook.Save("SqlScriptOperatorTypeExample.sql", saveOptions);

            // Output the results
            Console.WriteLine("SQL script has been saved successfully.");
        }
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


