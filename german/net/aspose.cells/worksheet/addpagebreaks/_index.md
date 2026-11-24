---
title: "Worksheet.AddPageBreaks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Fügt Seitenumbruch hinzu"
type: docs
url: /de/net/aspose.cells/worksheet/addpagebreaks/
---
## Worksheet.AddPageBreaks method

Fügt einen Seitenumbruch hinzu.

```csharp
public void AddPageBreaks(string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAddPageBreaksWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge horizontalen Seitenumbruch bei Zeile 1 (B2) hinzu
            worksheet.AddPageBreaks("B2");

            // Füge horizontalen Seitenumbruch bei Zeile 9 (B10) hinzu
            worksheet.AddPageBreaks("B10");

            // Überprüfe, ob der erste Seitenumbruch bei Zeile 1 hinzugefügt wurde
            Console.WriteLine("First page break row: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


