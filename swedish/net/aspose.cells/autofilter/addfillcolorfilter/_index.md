---
title: "AutoFilter.AddFillColorFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Lägger till ett fyllnadsfärgsfilter"
type: docs
url: /sv/net/aspose.cells/autofilter/addfillcolorfilter/
---
## AutoFilter.AddFillColorFilter method

Lägger till ett fyllnadsfärgsfilter.

```csharp
public void AddFillColorFilter(int fieldIndex, BackgroundType pattern, CellsColor foregroundColor, 
    CellsColor backgroundColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| mönster | BackgroundType | Bakgrundsmönstertypen. |
| foregroundColor | CellsColor | Förgrundsfärgen. |
| backgroundColor | CellsColor | Bakgrundsfärgen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFillColorFilterWithInt32BackgroundTypeCellsColorCDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med olika fyllningsfärger
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");
            
            // Applicera olika fyllningsfärger
            Style style1 = cells["A2"].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style1);
            
            Style style2 = cells["A3"].GetStyle();
            style2.ForegroundColor = Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style2);
            
            Style style3 = cells["A4"].GetStyle();
            style3.ForegroundColor = Color.Green;
            style3.Pattern = BackgroundType.Solid;
            cells["A4"].SetStyle(style3);

            // Skapa autofilter
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Skapa cellfärg för filtrering
            CellsColor filterColor = workbook.CreateCellsColor();
            filterColor.Color = Color.Red;
            
            // Applicera fyllningsfärgsfilter
            filter.AddFillColorFilter(0, BackgroundType.Solid, filterColor, filterColor);
            filter.Refresh();
            
            // Spara arbetsboken
            workbook.Save("AutoFilterFillColorDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BackgroundType](../../backgroundtype/)
* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


