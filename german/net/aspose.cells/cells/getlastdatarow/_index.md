---
title: "Cells.GetLastDataRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt den Index der letzten Zeile zurück, die in der angegebenen Spalte Daten enthält"
type: docs
url: /de/net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

Gibt den Index der letzten Zeile der Zelle zurück, die Daten in der angegebenen Spalte enthält.

```csharp
public int GetLastDataRow(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |

### Rückgabewert

Index der letzten Zeile.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetLastDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            
            // Ermitteln Sie die letzte Datenzeile in Spalte A (Index 0)
            int lastRow = worksheet.Cells.GetLastDataRow(0);
            
            // Gib das Ergebnis aus
            Console.WriteLine("Last data row in column A: " + lastRow);
            
            // Fügen Sie eine neue Zeile nach der letzten Datenzeile ein
            CellArea area = new CellArea();
            area.StartRow = lastRow + 1;
            area.EndRow = lastRow + 1;
            area.StartColumn = 0;
            area.EndColumn = 0;
            worksheet.Cells.InsertRange(area, 1, ShiftType.Down);
            
            // Daten zur neuen Zeile hinzufügen
            worksheet.Cells[lastRow + 2, 0].PutValue("New Data");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


