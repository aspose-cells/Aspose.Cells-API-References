---
title: "HighlightChangesOptions.HighlightChangesOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HighlightChangesOptions-Konstruktor. Stellt Optionen zum Hervorheben von Revisionen oder Änderungen von freigegebenen Excel-Dateien dar"
type: docs
url: /de/net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

Stellt Optionen zum Hervorheben von Revisionen oder Änderungen in freigegebenen Excel‑Dateien dar.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| highlightOnScreen | Boolean | Gibt an, ob Änderungen auf dem Bildschirm hervorgehoben werden. |
| listOnNewSheet | Boolean | Gibt an, ob Änderungen in einem neuen Arbeitsblatt aufgelistet werden. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie einige Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Erstelle HighlightChangesOptions mit booleschen Parametern
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            
            // Simuliere das Verfolgen von Änderungen (normalerweise hätten Sie tatsächliche Revisionen)
            Console.WriteLine("HighlightChangesOptions created with:");
            Console.WriteLine($"First parameter (show changes): {true}");
            Console.WriteLine($"Second parameter (changes on new sheet): {true}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("HighlightChangesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


