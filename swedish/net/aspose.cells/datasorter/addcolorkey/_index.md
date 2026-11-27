---
title: "DataSorter.AddColorKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter metod. Lägger till färgsorteringsnyckel"
type: docs
url: /sv/net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

Lägger till färgsorteringsnyckel.

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | Int32 | Den sorterade kolumnindexen (absolut position, kolumn A är 0, B är 1, ...) |
| typ | SortOnType | Den sorterade färgvärdestypen. |
| ordning | SortOrder | Sorteringsordningen. |
| färg | Färg | Den anpassade sorteringsfärgen. |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med färgade celler
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(7);
            
            // Applicera färger på celler.
            Style styleRed = workbook.CreateStyle();
            styleRed.ForegroundColor = Color.Red;
            styleRed.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(styleRed);
            
            Style styleBlue = workbook.CreateStyle();
            styleBlue.ForegroundColor = Color.Blue;
            styleBlue.Pattern = BackgroundType.Solid;
            worksheet.Cells["A3"].SetStyle(styleBlue);
            
            Style styleGreen = workbook.CreateStyle();
            styleGreen.ForegroundColor = Color.Green;
            styleGreen.Pattern = BackgroundType.Solid;
            worksheet.Cells["A4"].SetStyle(styleGreen);

            // Skapa datasortering och lägg till färgnyckel
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);

            // Sortera data
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));

            // Skriv ut de sorterade värdena (för demonstration)
            Console.WriteLine("Sorted values:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
            }
        }
    }
}
```

### Se även

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


