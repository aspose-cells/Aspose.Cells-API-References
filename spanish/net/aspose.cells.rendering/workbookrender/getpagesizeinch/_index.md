---
title: "WorkbookRender.GetPageSizeInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorkbookRender. Obtiene el tamaño de página en pulgadas de la imagen de salida"
type: docs
url: /es/net/aspose.cells.rendering/workbookrender/getpagesizeinch/
---
## WorkbookRender.GetPageSizeInch method

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

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test page size");
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            
            float[] pageSize = wr.GetPageSizeInch(0);
            Console.WriteLine($"Page size in inches: {pageSize[0]} x {pageSize[1]}");
        }
    }
}
```

### Ver también

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


