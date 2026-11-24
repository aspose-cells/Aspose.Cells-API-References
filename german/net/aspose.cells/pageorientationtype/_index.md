---
title: "Enum PageOrientationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PageOrientationType-Enum. Stellt Konstanten für die Druckausrichtung dar"
type: docs
url: /de/net/aspose.cells/pageorientationtype/
---
## PageOrientationType enumeration

Stellt Druckorientierungskonstanten dar.

```csharp
public enum PageOrientationType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Landscape | `0` | Querformat |
| Portrait | `1` | Hochformat |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageOrientationTypeDemo
    {
        public static void PageOrientationTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt in der Arbeitsmappe zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf das PageSetup-Objekt des Arbeitsblatts zu
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Setzen Sie die Seitenorientierung auf Querformat
            pageSetup.Orientation = PageOrientationType.Landscape;
            
            // Speichere die Arbeitsmappe in einer Datei
            workbook.Save("PageOrientationTypeExample_Landscape.xlsx");

            // Setzen Sie die Seitenorientierung auf Hochformat
            pageSetup.Orientation = PageOrientationType.Portrait;
            
            // Speichern Sie die Arbeitsmappe in einer anderen Datei
            workbook.Save("PageOrientationTypeExample_Portrait.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


