---
title: "SqlScriptSaveOptions.HasHeaderRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptSaveOptions-Eigenschaft. Gibt an, ob der Bereich eine Kopfzeile enthält"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/
---
## SqlScriptSaveOptions.HasHeaderRow property

Gibt an, ob der Bereich eine Kopfzeilenzeile enthält.

```csharp
public bool HasHeaderRow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kopfzeile und Beispieldaten hinzufügen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Bob");

            // SQL-Exportoptionen mit HasHeaderRow=true konfigurieren
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                HasHeaderRow = true,
                CreateTable = true
            };

            // Als SQL-Skript speichern
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script with header row exported successfully.");
        }
    }
}
```

### Siehe auch

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


