---
title: "CellWatchCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellWatchCollection-Methode. Fügt CellWatch mit einer Zeile und einer Spalte hinzu"
type: docs
url: /de/net/aspose.cells/cellwatchcollection/add/
---
## Add(int, int) {#add}

Fügt [`CellWatch`](../../cellwatch/) mit einer Zeile und einer Spalte hinzu.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Rückgabewert

Gibt die Position dieses Elements in der Sammlung zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rufe die CellWatchCollection aus dem Arbeitsblatt ab
            CellWatchCollection cellWatchCollection = worksheet.CellWatches;
            
            try
            {
                // Rufe die Add-Methode mit Zeilen- und Spaltenindizes (Int32, Int32) auf
                int index = cellWatchCollection.Add(5, 3); // Adding cell at row 6, column D (0-based)
                
                Console.WriteLine($"CellWatch added at index: {index}");
                
                // Überprüfe die hinzugefügte cell watch
                CellWatch cellWatch = cellWatchCollection[index];
                Console.WriteLine($"Watching cell: {cellWatch.Row},{cellWatch.Column}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("CellWatchCollectionMethodAddWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Fügt [`CellWatch`](../../cellwatch/) mit dem Namen der Zelle hinzu.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Der Name der Zelle. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige CellWatch-Instanzen hinzu.
            worksheet.CellWatches.Add("A1");
            worksheet.CellWatches.Add("B2");
            worksheet.CellWatches.Add("C3");
            
            // Zeige die Anzahl der cell watches an
            Console.WriteLine("Cell Watches Count: " + worksheet.CellWatches.Count);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


