---
title: "Cells.GetColumnWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Hämtar kolumnbredden"
type: docs
url: /sv/net/aspose.cells/cells/getcolumnwidth/
---
## GetColumnWidth(int, bool, CellsUnitType) {#getcolumnwidth_1}

Hämtar kolumnbredden.

```csharp
public double GetColumnWidth(int column, bool isOriginal, CellsUnitType unitType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindexet. |
| isOriginal | Boolean | Indikerar om den ursprungliga bredden hämtas. |
| unitType | CellsUnitType |  |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in kolumnbredd för kolumn 1 (0-baserat index)
            cells.SetColumnWidth(0, 20);

            // Hämta kolumnbredd i olika enheter och lägen
            double widthInPixels = cells.GetColumnWidth(0, true, CellsUnitType.Pixel);
            double widthInPoints = cells.GetColumnWidth(0, true, CellsUnitType.Point);
            double defaultWidth = cells.GetColumnWidth(0, false, CellsUnitType.Pixel);

            Console.WriteLine("Column width in pixels: " + widthInPixels);
            Console.WriteLine("Column width in points: " + widthInPoints);
            Console.WriteLine("Default column width: " + defaultWidth);
        }
    }
}
```

### Se även

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidth(int) {#getcolumnwidth}

Hämtar bredden (i tecken) för den angivna kolumnen i normal vy

```csharp
public double GetColumnWidth(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex |

### Returvärde

Kolumnbredd. För kalkylblad mäts kolumnbredd som antalet tecken av den maximala siffrabredden för siffrorna 0~9 som renderas i det normala stilens teckensnitt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in kolumnbredd för kolumnindex 255
            cells.SetColumnWidth(255, 20.86);

            // Hämta och visa kolumnbredden
            double columnWidth = cells.GetColumnWidth(255);
            Console.WriteLine("Column width at index 255: " + columnWidth);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


