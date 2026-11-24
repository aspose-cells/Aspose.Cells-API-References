---
title: "AutoFilter.AddFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Fügt einen Filter für eine Filterspalte hinzu"
type: docs
url: /de/net/aspose.cells/autofilter/addfilter/
---
## AutoFilter.AddFilter method

Fügt einen Filter für eine Filterspalte hinzu.

```csharp
public void AddFilter(int fieldIndex, string criteria)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| Kriterien | String | Die angegebenen Kriterien (ein String; zum Beispiel "101"). Sie können nur null sein oder einem der Zellwerte in dieser Spalte entsprechen. |

### Hinweise

MS Excel 2007 unterstützt Mehrfachauswahl in einer Filterspalte.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");
            worksheet.Cells["A6"].PutValue("Elderberry");
            
            // Auto-Filter-Bereich erstellen
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Hole den Auto-Filter
            AutoFilter filter = worksheet.AutoFilter;
            
            // Filter für Werte hinzufügen, die mit 'A' bzw. 'E' beginnen
            filter.AddFilter(0, "A*");
            filter.AddFilter(0, "E*");
            
            // Filter aktualisieren
            filter.Refresh();
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFilterAddFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


