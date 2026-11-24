---
title: "WorkbookSettings.Author"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Liest und setzt den Autor der Datei."
type: docs
url: /de/net/aspose.cells/workbooksettings/author/
---
## WorkbookSettings.Author property

Liest und setzt den Autor der Datei.

```csharp
public string Author { get; set; }
```

### Hinweise

Es ist nicht gesetzt, prüfen Sie zuerst [`Author`](../../../aspose.cells.properties/builtindocumentpropertycollection/author/), dann prüfen Sie den Benutzer der Umgebung.

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAuthorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;

            // Autor-Eigenschaft festlegen
            settings.Author = "John Doe";

            // Fügen Sie einige Beispieldaten hinzu, um die Arbeitsmappenfunktionalität zu demonstrieren
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Workbook");
            sheet.Cells["A2"].PutValue("Created by: " + settings.Author);
            sheet.Cells["A3"].PutValue(DateTime.Now.ToString());

            // Speichere die Arbeitsmappe
            workbook.Save("AuthorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


