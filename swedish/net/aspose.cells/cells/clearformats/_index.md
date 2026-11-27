---
title: "Cells.ClearFormats"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Rensar formatering av ett område"
type: docs
url: /sv/net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

Rensar formatering av ett område.

```csharp
public void ClearFormats(CellArea range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | CellArea | Område som ska rensas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearFormatsWithCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa exempeldata med formatering
            CellArea formatArea = new CellArea();
            formatArea.StartRow = 0;
            formatArea.StartColumn = 0;
            formatArea.EndRow = 2;
            formatArea.EndColumn = 2;

            // Tillämpa formatering på celler
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

            // Definiera rensningsområde
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 1;
            clearArea.StartColumn = 1;
            clearArea.EndRow = 1;
            clearArea.EndColumn = 1;

            try
            {
                // Rensa format från den centrala cellen
                cells.ClearFormats(clearArea);
                Console.WriteLine($"Cleared formats in area: Row {clearArea.StartRow}-{clearArea.EndRow}, Column {clearArea.StartColumn}-{clearArea.EndColumn}");
                
                // Uppdatera värdet i den rensade cellen för att visa effekten
                cells[1, 1].PutValue("Cleared Format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFormats: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("CellsMethodClearFormatsWithCellAreaDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearFormats(int, int, int, int) {#clearformats_1}

Rensar formatering av ett område.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradindex. |
| startColumn | Int32 | Startkolumnindex. |
| endRow | Int32 | Slutradindex. |
| endColumn | Int32 | Slutkolumnindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearFormatsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Tillämpa stilar på några celler
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            cells[0, 0].SetStyle(style);
            cells[0, 10].SetStyle(style);
            cells[10, 0].SetStyle(style);
            cells[10, 10].SetStyle(style);

            // Rensa format från ett specifikt område (rader 5-15, kolumner 5-15)
            cells.ClearFormats(5, 5, 15, 15);

            // Spara arbetsboken
            workbook.Save("ClearedFormats.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


