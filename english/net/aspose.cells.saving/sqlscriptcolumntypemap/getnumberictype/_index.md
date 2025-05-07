---
title: SqlScriptColumnTypeMap.GetNumbericType
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptColumnTypeMap method. Gets numeric type in the database
type: docs
url: /net/aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/
---
## SqlScriptColumnTypeMap.GetNumbericType method

Gets numeric type in the database.

```csharp
public virtual string GetNumbericType()
```

### Examples

```csharp
// Called: string numericType = columnTypeMap.GetNumbericType();
public static void Method_GetNumbericType()
        {
            // Create an instance of SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Demonstrate the usage of GetStringType and GetNumbericType methods
            string stringType = columnTypeMap.GetStringType();
            string numericType = columnTypeMap.GetNumbericType();

            // Output the results to the console
            Console.WriteLine("String Type in Database: " + stringType);
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Create an instance of SqlScriptSaveOptions and set the ColumnTypeMap
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };

            // Create a workbook and add some data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Save the workbook as SQL script using the save options
            workbook.Save("SqlScriptExample.sql", saveOptions);

            return;
        }
```

### See Also

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


