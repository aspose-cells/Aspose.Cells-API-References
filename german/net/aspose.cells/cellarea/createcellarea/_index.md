---
title: "CellArea.CreateCellArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellArea-Methode. Erstellt einen Zellbereich"
type: docs
url: /de/net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Erstellt einen Zellbereich.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Startzeile. |
| startColumn | Int32 | Die Startspalte. |
| endRow | Int32 | Die Endzeile. |
| endColumn | Int32 | Die Endspalte. |

### Rückgabewert

Gibt ein [`CellArea`](../) zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Zellen mit Beispieldaten füllen
            int[] values = { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
            for (int i = 0; i < values.Length; i++)
            {
                cells[i, i / 3].PutValue(values[i]);
            }

            // Erstellen und konfigurieren Sie den Datensortierer
            DataSorter sorter = wb.DataSorter;
            sorter.Clear();
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 2;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 0;

            // Sortieren Sie mit CreateCellArea und Int32-Parametern
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));

            // Sortierte Werte ausgeben
            Console.WriteLine("Sorted values:");
            for (int i = 0; i < 9; i++)
            {
                Console.WriteLine(cells[i, 2 - i / 3].IntValue);
            }
        }
    }
}
```

### Siehe auch

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Erstellt einen Zellbereich.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startCellName | String | Die Zelle oben links des Bereichs. |
| endCellName | String | Die Zelle unten rechts des Bereichs. |

### Rückgabewert

Gibt ein [`CellArea`](../) zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Füllen Sie einige Daten in Spalte A ein
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Data {i}");
            }

            // Erstellen Sie einen Zellbereich von B1 bis B10
            CellArea area = CellArea.CreateCellArea("B1", "B10");
            
            // Bereich einfügen und Zellen nach unten verschieben
            cells.InsertRange(area, ShiftType.Down);
            
            // Verifizieren Sie den Vorgang, indem Sie die Zellwerte prüfen
            Console.WriteLine("Inserted range from B1 to B10. Total rows: " + cells.Rows.Count);
        }
    }
}
```

### Siehe auch

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


