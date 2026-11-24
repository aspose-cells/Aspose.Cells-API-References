---
title: "Cells.ClearRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Löscht Inhalte und Formatierung eines Bereichs"
type: docs
url: /de/net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

Löscht Inhalt und Formatierung eines Bereichs.

```csharp
public void ClearRange(CellArea range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | CellArea | Zu löschender Bereich. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zellen mit Beispieldaten füllen
            for (int row = 0; row <= 2; row++)
            {
                for (int col = 0; col <= 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data_{row}_{col}";
                }
            }

            // Definiere den zu löschenden CellArea (Zeilen 0-2, Spalten 0-2)
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 0;
            clearArea.EndRow = 2;
            clearArea.StartColumn = 0;
            clearArea.EndColumn = 2;

            try
            {
                // Lösche den angegebenen Bereich
                worksheet.Cells.ClearRange(clearArea);
                Console.WriteLine("Cleared cells in range: Rows 0-2, Columns 0-2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearRange method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("CellsMethodClearRangeWithCellAreaDemo.xlsx");
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

## ClearRange(int, int, int, int) {#clearrange_1}

Löscht Inhalt und Formatierung eines Bereichs.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
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
    public class CellsMethodClearRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Fülle einige Testdaten ein
            cells[0, 0].PutValue(1);
            cells[0, 16383].PutValue(2);
            cells[1048575, 0].PutValue(3);
            cells[1048575, 16383].PutValue(4);

            // Lösche den gesamten Arbeitsblattbereich
            cells.ClearRange(0, 0, 1048575, 16383);

            // Speichere die Arbeitsmappe
            workbook.Save("ClearRangeDemo.xlsx");

            Console.WriteLine("ClearRange demo executed successfully.");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


