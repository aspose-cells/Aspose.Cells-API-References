---
title: "Cells.InsertRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Fügt eine neue Zeile in das Arbeitsblatt ein"
type: docs
url: /de/net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

Fügt eine neue Zeile in das Arbeitsblatt ein.

```csharp
public void InsertRow(int rowIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Zeilenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet sheet = workbook.Worksheets[0];
            
            // Zellsammlung abrufen
            Cells cells = sheet.Cells;
            
            // Beispieldaten in Zeile 6 einfügen
            cells[6, 0].PutValue("Original Row 6");
            cells[6, 1].PutValue(100);
            
            // Beispieldaten in Zeile 7 einfügen
            cells[7, 0].PutValue("Original Row 7");
            cells[7, 1].PutValue(200);
            
            // Füge eine neue Zeile bei Index 7 ein (schiebt die vorhandene Zeile 7 nach unten)
            cells.InsertRow(7);
            
            // Daten zur neu eingefügten Zeile hinzufügen
            cells[7, 0].PutValue("New Inserted Row");
            cells[7, 1].PutValue(150);
            
            // Speichere die Arbeitsmappe
            workbook.Save("InsertRowDemo.xlsx");
            
            Console.WriteLine("Row inserted successfully at index 7.");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


