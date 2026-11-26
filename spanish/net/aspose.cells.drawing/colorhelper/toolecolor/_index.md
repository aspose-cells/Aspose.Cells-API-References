---
title: "ColorHelper.ToOleColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ColorHelper. Convierte color a OLE_COLOR"
type: docs
url: /es/net/aspose.cells.drawing/colorhelper/toolecolor/
---
## ColorHelper.ToOleColor method

Convertir color a OLE_COLOR

```csharp
public static int ToOleColor(Color color, Workbook workbook)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | Color | El objeto Color. |
| libro de trabajo | Libro de trabajo |  |

### Valor de retorno

El valor de OLE_COLOR

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ColorHelperMethodToOleColorWithColorWorkbookDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                Color color = Color.Red;

                int oleColor = ColorHelper.ToOleColor(color, workbook);

                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("OLE Color Demonstration");
                
                Style style = workbook.CreateStyle();
                style.ForegroundColor = ColorHelper.FromOleColor(oleColor);
                style.Pattern = BackgroundType.Solid;
                cell.SetStyle(style);

                Console.WriteLine($"Converted OLE Color: {oleColor}");
                Console.WriteLine("Cell A1 background set using converted color.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ToOleColorWithColorWorkbookDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../../../aspose.cells/workbook/)
* class [ColorHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


