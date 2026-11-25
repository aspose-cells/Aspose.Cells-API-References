---
title: "ColorHelper.FromOleColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ColorHelper. Converte OLE_COLOR"
type: docs
url: /it/net/aspose.cells.drawing/colorhelper/fromolecolor/
---
## ColorHelper.FromOleColor method

Converti OLE_COLOR.

```csharp
public static Color FromOleColor(int oleColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oleColor | Int32 | Il valore di OLE_COLOR. |

### Valore di ritorno

L'oggetto Color.

### Esempi

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
                
                // Applica il colore allo sfondo della cella
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

### Vedi anche

* class [ColorHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


