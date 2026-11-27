---
title: "ColorHelper.FromOleColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ColorHelper-metod. Konvertera OLE_COLOR"
type: docs
url: /sv/net/aspose.cells.drawing/colorhelper/fromolecolor/
---
## ColorHelper.FromOleColor method

Konvertera OLE_COLOR.

```csharp
public static Color FromOleColor(int oleColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oleColor | Int32 | Värdet av OLE_COLOR. |

### Returvärde

Färgobjektet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ColorHelperMethodFromOleColorWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int oleColor = 0x00FF0000; // OLE color for blue in BGR format
            
            try
            {
                Color convertedColor = ColorHelper.FromOleColor(oleColor);
                
                // Applicera färg på cellbakgrund
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Color converted from OLE");
                Style style = cell.GetStyle();
                style.ForegroundColor = convertedColor;
                style.Pattern = BackgroundType.Solid;
                cell.SetStyle(style);
                
                Console.WriteLine($"Converted OLE color {oleColor:X} to RGB: {convertedColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            
            workbook.Save("ColorHelperMethodFromOleColorWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [ColorHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


