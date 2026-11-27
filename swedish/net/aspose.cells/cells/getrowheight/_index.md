---
title: "Cells.GetRowHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Hämtar radhöjden"
type: docs
url: /sv/net/aspose.cells/cells/getrowheight/
---
## GetRowHeight(int, bool, CellsUnitType) {#getrowheight_1}

Hämtar radens höjd.

```csharp
public double GetRowHeight(int row, bool isOriginal, CellsUnitType unitType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| isOriginal | Boolean | Anger om den returnerar den ursprungliga radhöjden eller 0 för dold rad. |
| unitType | CellsUnitType | Enhetstyp för det returnerade höjdvärdet |

### Returvärde

Radhöjd

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in radhöjden för rad 3 (20 pixlar)
            worksheet.Cells.SetRowHeightPixel(3, 20);
            
            // Hämta radhöjd i olika enheter
            double heightInPixels = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Pixel);
            double heightInPoints = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Point);
            
            // Skriv ut resultaten
            Console.WriteLine("Row height in pixels: " + heightInPixels);
            Console.WriteLine("Row height in points: " + heightInPoints);
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

## GetRowHeight(int) {#getrowheight}

Hämtar höjden på en specificerad rad, i enhet punkter.

```csharp
public double GetRowHeight(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex |

### Returvärde

Radhöjd

### Exempel

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

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


