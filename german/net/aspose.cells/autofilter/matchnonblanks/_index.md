---
title: "AutoFilter.MatchNonBlanks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Alle nichtleeren Zellen in der Liste abgleichen"
type: docs
url: /de/net/aspose.cells/autofilter/matchnonblanks/
---
## AutoFilter.MatchNonBlanks method

Alle nicht-leeren Zellen in der Liste abgleichen.

```csharp
public void MatchNonBlanks(int fieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodMatchNonBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten mit einigen leeren Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(""); // Blank cell
            worksheet.Cells["B3"].PutValue(5);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(8);
            worksheet.Cells["A5"].PutValue(""); // Blank cell
            worksheet.Cells["B5"].PutValue(12);

            // Auto-Filter anwenden, um nur nicht-leere Zellen in Spalte A (Index 0) anzuzeigen
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.MatchNonBlanks(0);
            worksheet.AutoFilter.Refresh();

            // Speichere die Arbeitsmappe
            workbook.Save("FilterNonBlanks.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


