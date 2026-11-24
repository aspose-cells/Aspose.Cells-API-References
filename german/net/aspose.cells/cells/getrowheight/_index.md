---
title: "Cells.GetRowHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Ermittelt die Zeilenhöhe"
type: docs
url: /de/net/aspose.cells/cells/getrowheight/
---
## GetRowHeight(int, bool, CellsUnitType) {#getrowheight_1}

Gibt die Zeilenhöhe zurück.

```csharp
public double GetRowHeight(int row, bool isOriginal, CellsUnitType unitType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| isOriginal | Boolean | Ob die ursprüngliche Zeilenhöhe oder 0 für eine ausgeblendete Zeile zurückgegeben wird. |
| unitType | CellsUnitType | Einheitstyp des zurückgegebenen Höhenwerts |

### Rückgabewert

Zeilenhöhe

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze die Zeilenhöhe für Zeile 3 (20 Pixel)
            worksheet.Cells.SetRowHeightPixel(3, 20);
            
            // Erhalte die Zeilenhöhe in verschiedenen Einheiten
            double heightInPixels = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Pixel);
            double heightInPoints = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Point);
            
            // Ergebnisse ausgeben
            Console.WriteLine("Row height in pixels: " + heightInPixels);
            Console.WriteLine("Row height in points: " + heightInPoints);
        }
    }
}
```

### Siehe auch

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRowHeight(int) {#getrowheight}

Gibt die Höhe einer angegebenen Zeile in Punkten zurück.

```csharp
public double GetRowHeight(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex |

### Rückgabewert

Höhe der Zeile

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets["Sheet1"];
            Cells cells = ws.Cells;
            
            string strText = "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.";
            cells[0, 0].PutValue(strText);
            
            Style style = cells[0, 0].GetStyle();
            style.IsTextWrapped = true;
            cells[0, 0].SetStyle(style);
            
            ws.Cells.SetColumnWidth(0, 50);
            ws.AutoFitRows();
            
            double rowHeight = cells.GetRowHeight(0);
            Console.WriteLine("Row height: " + rowHeight);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


