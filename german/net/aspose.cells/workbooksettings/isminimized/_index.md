---
title: "WorkbookSettings.IsMinimized"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob die erzeugte Tabelle minimiert geöffnet wird"
type: docs
url: /de/net/aspose.cells/workbooksettings/isminimized/
---
## WorkbookSettings.IsMinimized property

Gibt an, ob das erzeugte Tabellenblatt minimiert geöffnet wird.

```csharp
public bool IsMinimized { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsMinimizedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Setze die IsMinimized-Eigenschaft auf true
            workbook.Settings.IsMinimized = true;

            // Speichere die Arbeitsmappe
            workbook.Save("IsMinimizedDemo.xlsx");

            // Laden Sie die gespeicherte Arbeitsmappe, um die Eigenschaft zu überprüfen
            Workbook loadedWorkbook = new Workbook("IsMinimizedDemo.xlsx");

            // Gib den Wert der IsMinimized-Eigenschaft aus
            Console.WriteLine("Workbook IsMinimized property: " + loadedWorkbook.Settings.IsMinimized);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


