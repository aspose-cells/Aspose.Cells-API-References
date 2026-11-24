---
title: "Cells.IsBlankColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Prüft, ob die angegebene Spalte leer ist und keine Daten enthält"
type: docs
url: /de/net/aspose.cells/cells/isblankcolumn/
---
## Cells.IsBlankColumn method

Prüft, ob die angegebene Spalte leer ist (enthält keine Daten).

```csharp
public bool IsBlankColumn(int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | der Spaltenindex |

### Rückgabewert

wahr, wenn die angegebene Spalte keine Daten enthält

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsBlankColumnWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prüfe, ob Spalte 2 leer ist (sollte für ein neues Arbeitsblatt wahr sein)
            Console.WriteLine("Is column 2 blank? " + worksheet.Cells.IsBlankColumn(1));

            // Daten zu Spalte 2 hinzufügen
            worksheet.Cells["B1"].PutValue("Test Data");

            // Erneut prüfen (sollte jetzt false sein)
            Console.WriteLine("Is column 2 blank after adding data? " + worksheet.Cells.IsBlankColumn(1));

            // Erstelle ein weiteres Arbeitsblatt mit vollständig leeren Spalten
            Worksheet worksheet2 = workbook.Worksheets.Add("BlankSheet");

            // Prüfe eine Spalte im leeren Arbeitsblatt (sollte true sein)
            Console.WriteLine("Is column 3 blank in new sheet? " + worksheet2.Cells.IsBlankColumn(2));
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


