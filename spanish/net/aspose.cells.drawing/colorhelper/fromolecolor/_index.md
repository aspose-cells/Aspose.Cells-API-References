---
title: "ColorHelper.FromOleColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ColorHelper. Convierte OLE_COLOR"
type: docs
url: /es/net/aspose.cells.drawing/colorhelper/fromolecolor/
---
## ColorHelper.FromOleColor method

Convertir OLE_COLOR.

```csharp
public static Color FromOleColor(int oleColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oleColor | Int32 | El valor de OLE_COLOR. |

### Valor de retorno

El objeto Color.

### Ejemplos

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
                
                // Aplicar color al fondo de la celda
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

### Ver también

* class [ColorHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


