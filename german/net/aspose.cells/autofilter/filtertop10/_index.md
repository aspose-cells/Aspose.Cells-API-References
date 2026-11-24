---
title: "AutoFilter.FilterTop10"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Filtert die Top‑10‑Einträge in der Liste"
type: docs
url: /de/net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Filtere die obersten 10 Elemente in der Liste

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| isTop | Boolean | Gibt an, ob der Filter von oben oder unten kommt |
| isPercent | Boolean | Gibt an, ob die Elemente Prozent oder Anzahl sind |
| itemCount | Int32 | Die Anzahl der Elemente |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterTop10WithInt32BooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen (5 Zeilen x 3 Spalten mit numerischen Werten)
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Numbers");
            cells["A2"].PutValue(50);
            cells["A3"].PutValue(30);
            cells["A4"].PutValue(80);
            cells["A5"].PutValue(20);
            cells["A6"].PutValue(90);

            // Autofilterbereich festlegen
            worksheet.AutoFilter.Range = "A1:A6";

            // Top‑10‑Filter anwenden (zeigt die obersten 2 Elemente)
            worksheet.AutoFilter.FilterTop10(0, true, false, 2);

            // Filter aktualisieren
            worksheet.AutoFilter.Refresh();

            // Speichere die Arbeitsmappe
            workbook.Save("FilterTop10Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


