---
title: "Cells.ClearContents"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Löscht den Inhalt eines Bereichs"
type: docs
url: /de/net/aspose.cells/cells/clearcontents/
---
## ClearContents(CellArea) {#clearcontents}

Löscht den Inhalt eines Bereichs.

```csharp
public void ClearContents(CellArea range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | CellArea | Zu löschender Bereich. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearContentsWithCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fülle einige Daten in einem Zellbereich
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Data_{row}_{col}");
                }
            }

            Console.WriteLine("Before ClearContents:");
            PrintCellAreaContents(cells, area);

            // Lösche den Inhalt des Zellbereichs
            cells.ClearContents(area);

            Console.WriteLine("\nAfter ClearContents:");
            PrintCellAreaContents(cells, area);
        }

        private static void PrintCellAreaContents(Cells cells, CellArea area)
        {
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    Console.Write(cells[row, col].StringValue + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearContents(int, int, int, int) {#clearcontents_1}

Löscht den Inhalt eines Bereichs.

```csharp
public void ClearContents(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Startzeilenindex. |
| startColumn | Int32 | Startspaltenindex. |
| endRow | Int32 | Endzeilenindex. |
| endColumn | Int32 | Endspaltenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearContentsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Füllen Sie einige Zellen mit Werten
            cells[0, 0].PutValue("Value A1");
            cells[0, 1].PutValue("Value B1");
            cells[1, 0].PutValue("Value A2");
            cells[1, 1].PutValue("Value B2");

            // Zeige ursprüngliche Werte an
            Console.WriteLine("Before ClearContents:");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Lösche den Inhalt von Zellen im Bereich (0,1) bis (1,1)
            cells.ClearContents(0, 1, 1, 1);

            // Zeige Werte nach dem Löschen an
            Console.WriteLine("\nAfter ClearContents(0, 1, 1, 1):");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Speichere die Arbeitsmappe
            workbook.Save("ClearContentsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


