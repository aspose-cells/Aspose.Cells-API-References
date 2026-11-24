---
title: "SqlScriptSaveOptions.IdName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptSaveOptions-Eigenschaft. Gibt den Namen der ID-Spalte zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptsaveoptions/idname/
---
## SqlScriptSaveOptions.IdName property

Liest und setzt den Namen der ID-Spalte.

```csharp
public string IdName { get; set; }
```

### Hinweise

Wenn diese Eigenschaft gesetzt ist, wird eine Spalte mit automatisch inkrementierendem Ganzzahlwert eingefügt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyIdNameDemo
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

            // SQL-Exportoptionen mit IdName konfigurieren
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Als SQL-Skript speichern
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script exported with IdName property");
        }
    }
}
```

### Siehe auch

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


