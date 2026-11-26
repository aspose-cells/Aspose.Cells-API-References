---
title: "SheetRender.PageScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SheetRender. Obtiene la escala de página calculada de la hoja. Devuelve la escala establecida si Zoom está configurado. De lo contrario, devuelve la escala calculada según FitToPagesWide y FitToPagesTall"
type: docs
url: /es/net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

Obtiene la escala de página calculada de la hoja. Devuelve la escala establecida si [`Zoom`](../../../aspose.cells/pagesetup/zoom/) está configurado. De lo contrario, devuelve la escala calculada según [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) y [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/).

```csharp
public double PageScale { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageScaleDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue($"Item {i + 1}");
                sheet.Cells[i, 1].PutValue((i + 1) * 10);
            }

            // Crear opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Crear renderizado de hoja
            SheetRender sheetRender = new SheetRender(sheet, options);
            
            // Obtener y mostrar la escala de página calculada
            double pageScale = sheetRender.PageScale;
            Console.WriteLine($"Calculated Page Scale: {pageScale}");
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


