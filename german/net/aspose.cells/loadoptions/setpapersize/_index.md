---
title: "LoadOptions.SetPaperSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions‑Methode. Setzt die Standard‑Papiergröße für den Druck aus den Einstellungen des Standard‑Druckers"
type: docs
url: /de/net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

Setzt die Standard‑Papiergröße für den Druck aus den Einstellungen des Standard‑Druckers.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | PaperSizeType | Die Standard‑Papiergröße. |

### Hinweise

Wenn keine Einstellung zur Papiergröße vorhanden ist, verwendet MS Excel die Einstellung des Standarddruckers.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsMethodSetPaperSizeWithPaperSizeTypeDemo
    {
        public static void Run()
        {
            // Ladeoptionen erstellen und Papiergröße auf A5 setzen
            LoadOptions options = new LoadOptions();
            options.SetPaperSize(PaperSizeType.PaperA5);

            // Arbeitsmappe mit den angegebenen Optionen laden
            Workbook workbook = new Workbook("example.xlsx", options);
            
            // Verifizieren, dass die Papiergröße korrekt gesetzt ist
            Console.WriteLine("Paper size of first worksheet: " + workbook.Worksheets[0].PageSetup.PaperSize);
        }
    }
}
```

### Siehe auch

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


