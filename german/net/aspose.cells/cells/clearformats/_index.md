---
title: "Cells.ClearFormats"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Löscht die Formatierung eines Bereichs."
type: docs
url: /de/net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

Löscht die Formatierung eines Bereichs.

```csharp
public void ClearFormats(CellArea range)
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

    public class CellsMethodClearFormatsWithCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten mit Formatierung erstellen.
            CellArea formatArea = new CellArea();
            formatArea.StartRow = 0;
            formatArea.StartColumn = 0;
            formatArea.EndRow = 2;
            formatArea.EndColumn = 2;

            // Formatierung auf Zellen anwenden.
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            
            for (int row = formatArea.StartRow; row <= formatArea.EndRow; row++)
            {
                for (int col = formatArea.StartColumn; col <= formatArea.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Formatted {row},{col}");
                    cells[row, col].SetStyle(style);
                }
            }

            // Klaren Bereich definieren
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 1;
            clearArea.StartColumn = 1;
            clearArea.EndRow = 1;
            clearArea.EndColumn = 1;

            try
            {
                // Formate aus der mittleren Zelle löschen
                cells.ClearFormats(clearArea);
                Console.WriteLine($"Cleared formats in area: Row {clearArea.StartRow}-{clearArea.EndRow}, Column {clearArea.StartColumn}-{clearArea.EndColumn}");
                
                // Aktualisieren Sie den Wert der gelöschten Zelle, um den Effekt zu zeigen
                cells[1, 1].PutValue("Cleared Format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFormats: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("CellsMethodClearFormatsWithCellAreaDemo.xlsx");
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

## ClearFormats(int, int, int, int) {#clearformats_1}

Löscht die Formatierung eines Bereichs.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
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
    public class CellsMethodClearFormatsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Stile auf einige Zellen anwenden
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            cells[0, 0].SetStyle(style);
            cells[0, 10].SetStyle(style);
            cells[10, 0].SetStyle(style);
            cells[10, 10].SetStyle(style);

            // Formate aus einem bestimmten Bereich (Zeilen 5-15, Spalten 5-15) löschen
            cells.ClearFormats(5, 5, 15, 15);

            // Speichere die Arbeitsmappe
            workbook.Save("ClearedFormats.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


