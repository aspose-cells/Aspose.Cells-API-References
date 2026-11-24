---
title: "Enum GridlineType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridlineType Aufzählung. Enumeriert den Gitterlinientyp."
type: docs
url: /de/net/aspose.cells/gridlinetype/
---
## GridlineType enumeration

Enumeriert den Gitterlinientyp.

```csharp
public enum GridlineType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Dotted | `0` | Stellt eine gepunktete Linie dar. |
| Hair | `1` | Stellt eine Feinlinie dar. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGridlineTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle Speicheroptionen und setze den Gitterlinientyp.
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.GridlineType = GridlineType.Dotted;
            
            // Füge einige Beispieldaten hinzu, um Gitterlinien zu sehen.
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            // Speichere das Workbook mit den Speicheroptionen.
            workbook.Save("GridlineTypeDemo.docx", saveOptions);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


