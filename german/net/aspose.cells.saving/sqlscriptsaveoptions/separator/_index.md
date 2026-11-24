---
title: "SqlScriptSaveOptions.Separator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptSaveOptions-Eigenschaft. Gibt das Zeichen-Trennzeichen des SQL-Skripts zurück und legt es fest"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptsaveoptions/separator/
---
## SqlScriptSaveOptions.Separator property

Liest und setzt das Zeichen‑Trennzeichen des SQL‑Skripts.

```csharp
public char Separator { get; set; }
```

### Hinweise

Kann nur ' ' oder '\n' sein. Wenn die

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John");

            // SQL-Speicheroptionen mit benutzerdefiniertem Trennzeichen konfigurieren
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                Separator = ';',
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Speichere mit benutzerdefiniertem Trennzeichen
            workbook.Save("SqlScriptWithSeparator.sql", saveOptions);

            Console.WriteLine("SQL script saved with custom separator.");
        }
    }
}
```

### Siehe auch

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


