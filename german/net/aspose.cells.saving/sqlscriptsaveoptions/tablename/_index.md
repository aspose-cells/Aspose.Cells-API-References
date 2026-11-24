---
title: "SqlScriptSaveOptions.TableName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptSaveOptions-Eigenschaft. Liest und setzt den Tabellennamen"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptsaveoptions/tablename/
---
## SqlScriptSaveOptions.TableName property

Liest und setzt den Tabellennamen.

```csharp
public string TableName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyTableNameDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch mit einigen Daten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // SQL‑Speicheroptionen mit benutzerdefiniertem Tabellennamen konfigurieren
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions();
            saveOptions.TableName = "Employees"; // Demonstrating TableName property
            saveOptions.CreateTable = true;
            saveOptions.OperatorType = SqlScriptOperatorType.Insert;

            // Als SQL-Skript speichern
            workbook.Save("output.sql", saveOptions);

            Console.WriteLine("SQL Script generated with table name 'Employees'");
        }
    }
}
```

### Siehe auch

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


