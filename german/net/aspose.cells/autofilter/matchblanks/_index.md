---
title: "AutoFilter.MatchBlanks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Alle leeren Zellen in der Liste abgleichen"
type: docs
url: /de/net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Alle leeren Zellen in der Liste abgleichen.

```csharp
public void MatchBlanks(int fieldIndex)
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
    public class AutoFilterMethodMatchBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten mit einigen leeren Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // C2 leer lassen
            
            worksheet.Cells["A3"].PutValue("Data3");
            // B3 leer lassen
            worksheet.Cells["C3"].PutValue("Data6");
            
            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:C3";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Filtern, um nur Zeilen mit leeren Zellen in Spalte 3 (C) anzuzeigen
            filter.MatchBlanks(2); // Column index is 0-based
            
            // Filter aktualisieren
            filter.Refresh();
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFilterMatchBlanksDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


