---
title: "WorkbookSettings.PaperSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Ruft die Standard-Druckpapiergröße ab und legt sie fest"
type: docs
url: /de/net/aspose.cells/workbooksettings/papersize/
---
## WorkbookSettings.PaperSize property

Liest und setzt die Standard-Papiergröße für den Druck.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Hinweise

Wenn keine Einstellung zur Papiergröße vorhanden ist, verwendet MS Excel die Einstellung des Standarddruckers.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze die Papiergröße auf A5
            workbook.Settings.PaperSize = PaperSizeType.PaperA5;
            
            // Überprüfe, ob die Papiergröße im ersten Arbeitsblatt korrekt eingestellt ist
            Console.WriteLine("Paper size: " + workbook.Worksheets[0].PageSetup.PaperSize);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


