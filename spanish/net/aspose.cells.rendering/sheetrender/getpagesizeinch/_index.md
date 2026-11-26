---
title: "SheetRender.GetPageSizeInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SheetRender. Obtenga el tamaño de página en pulgadas de la imagen de salida"
type: docs
url: /es/net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

Obtener el tamaño de página en pulgadas de la imagen de salida.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | El índice de página se basa en cero. |

### Valor de retorno

Tamaño de la imagen, [0] para el ancho y [1] para la altura

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.PrintArea = "A1:D10";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);
            float[] pageSize = sheetRender.GetPageSizeInch(0);
            
            Console.WriteLine($"Page Size (Inches): Width={pageSize[0]}, Height={pageSize[1]}");
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


