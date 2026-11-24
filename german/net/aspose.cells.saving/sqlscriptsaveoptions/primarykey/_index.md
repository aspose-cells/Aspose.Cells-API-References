---
title: "SqlScriptSaveOptions.PrimaryKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptSaveOptions-Eigenschaft. Gibt an, welche Spalte der Primärschlüssel der Datentabelle ist"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptsaveoptions/primarykey/
---
## SqlScriptSaveOptions.PrimaryKey property

Gibt an, welche Spalte der Primärschlüssel der Datentabelle ist.

```csharp
public int PrimaryKey { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyPrimaryKeyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // SQL-Exportoptionen mit PrimaryKey auf die erste Spalte (0) setzen
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                PrimaryKey = 0,
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Als SQL-Skript speichern
            workbook.Save("EmployeesExport.sql", saveOptions);

            Console.WriteLine("SQL script exported with PrimaryKey set to column 0 (ID)");
        }
    }
}
```

### Siehe auch

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


