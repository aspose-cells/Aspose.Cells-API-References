---
title: "Clase ColorHelper"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ColorHelper. Proporciona funciones auxiliares sobre el color"
type: docs
url: /es/net/aspose.cells.drawing/colorhelper/
---
## ColorHelper class

Proporciona funciones auxiliares sobre el color.

```csharp
public class ColorHelper
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [FromOleColor](../../aspose.cells.drawing/colorhelper/fromolecolor/)(int) | Convertir OLE_COLOR. |
| static [ToOleColor](../../aspose.cells.drawing/colorhelper/toolecolor/)(Color, Workbook) | Convertir color a OLE_COLOR |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassColorHelperDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Convertir color OLE a System.Drawing.Color (Verde)
            int oleGreen = 0x00FF00;
            Color colorFromOle = ColorHelper.FromOleColor(oleGreen);

            // Aplicar el color convertido al fondo de la celda A1
            Cell cellA1 = worksheet.Cells["A1"];
            Style styleA1 = cellA1.GetStyle();
            styleA1.ForegroundColor = colorFromOle;
            styleA1.Pattern = BackgroundType.Solid;
            cellA1.SetStyle(styleA1);

            // Convertir System.Drawing.Color de nuevo a color OLE
            int convertedOle = ColorHelper.ToOleColor(colorFromOle, workbook);

            // Convertir el resultado OLE de nuevo a Color (verificación)
            Color colorFromConvertedOle = ColorHelper.FromOleColor(convertedOle);

            // Aplicar el color reconvertido al fondo de la celda A2
            Cell cellA2 = worksheet.Cells["A2"];
            Style styleA2 = cellA2.GetStyle();
            styleA2.ForegroundColor = colorFromConvertedOle;
            styleA2.Pattern = BackgroundType.Solid;
            cellA2.SetStyle(styleA2);

            // Guardar el libro de trabajo modificado
            workbook.Save("DrawingClassColorHelperDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


