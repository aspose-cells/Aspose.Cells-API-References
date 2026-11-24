---
title: "WorkbookSettings.UpdateLinksType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an und legt fest, wie externe Links beim Öffnen der Arbeitsmappe aktualisiert werden"
type: docs
url: /de/net/aspose.cells/workbooksettings/updatelinkstype/
---
## WorkbookSettings.UpdateLinksType property

Liest und setzt, wie externe Links beim Öffnen der Arbeitsmappe aktualisiert werden.

```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateLinksTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze UpdateLinksType auf Never
            workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Lade die gespeicherte Arbeitsmappe, um die Einstellung zu überprüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Gib den UpdateLinksType-Wert aus
            Console.WriteLine("UpdateLinksType: " + loadedWorkbook.Settings.UpdateLinksType);
        }
    }
}
```

### Siehe auch

* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


