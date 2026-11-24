---
title: "Cells.RemoveDuplicates"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Entfernt doppelte Zeilen im Blatt"
type: docs
url: /de/net/aspose.cells/cells/removeduplicates/
---
## RemoveDuplicates() {#removeduplicates}

Entfernt doppelte Zeilen im Blatt.

```csharp
public void RemoveDuplicates()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Füllt Zellen mit einigen doppelten Werten
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    // Erstellt Duplikate in jeder zweiten Zeile
                    cells[i, j].PutValue(i % 2 == 0 ? "Duplicate" : $"Unique_{i}_{j}");
                }
            }

            Console.WriteLine($"Before RemoveDuplicates: {cells.Count} cells");
            
            // Entfernt doppelte Werte
            cells.RemoveDuplicates();

            Console.WriteLine($"After RemoveDuplicates: {cells.Count} cells");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int) {#removeduplicates_1}

Entfernt doppelte Werte im Bereich.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Startzeile. |
| startColumn | Int32 | Die Startspalte |
| endRow | Int32 | Der Endzeilenindex. |
| endColumn | Int32 | Der Endspaltenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Füge Beispieldaten mit Duplikaten hinzu
            cells["A1"].PutValue("Apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("Apple");
            cells["A4"].PutValue("Banana");
            cells["A5"].PutValue("Orange");

            // Entfernt Duplikate aus Spalte A (0-basierter Index)
            cells.RemoveDuplicates(0, 0, 5, 0);

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

---

## RemoveDuplicates(int, int, int, int, bool, int[]) {#removeduplicates_2}

Entfernt doppelte Daten des Bereichs.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn, 
    bool hasHeaders, int[] columnOffsets)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Startzeile. |
| startColumn | Int32 | Die Startspalte |
| endRow | Int32 | Der Endzeilenindex. |
| endColumn | Int32 | Der Endspaltenindex. |
| hasHeaders | Boolean | Gibt an, ob der Bereich Kopfzeilen enthält. |
| columnOffsets | Int32[] | Die Spaltenversätze. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32BooleanIntDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fülle Beispieldaten mit Duplikaten
            cells[0, 0].PutValue("ID");
            cells[0, 1].PutValue("Name");
            cells[0, 2].PutValue("Age");
            
            cells[1, 0].PutValue(1);
            cells[1, 1].PutValue("John");
            cells[1, 2].PutValue(30);

            cells[2, 0].PutValue(2);
            cells[2, 1].PutValue("Jane");
            cells[2, 2].PutValue(25);

            cells[3, 0].PutValue(1); // Duplicate ID
            cells[3, 1].PutValue("John"); // Duplicate Name
            cells[3, 2].PutValue(35);

            cells[4, 0].PutValue(3);
            cells[4, 1].PutValue("Bob");
            cells[4, 2].PutValue(40);

            try
            {
                // Entfernt Duplikate aus Zeilen 1-4 (0-basiert), Spalten 0-2
                // Duplikate anhand der ersten beiden Spalten (ID und Name) prüfen
                cells.RemoveDuplicates(1, 0, 4, 2, true, new int[] { 0, 1 });

                Console.WriteLine("Duplicates removed successfully. Remaining rows: " + (cells.MaxDataRow + 1));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveDuplicates method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("RemoveDuplicatesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


