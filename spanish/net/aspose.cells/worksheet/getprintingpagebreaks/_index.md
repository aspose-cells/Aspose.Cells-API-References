---
title: "Worksheet.GetPrintingPageBreaks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Obtiene saltos de página automáticos"
type: docs
url: /es/net/aspose.cells/worksheet/getprintingpagebreaks/
---
## Worksheet.GetPrintingPageBreaks method

Obtiene los saltos de página automáticos.

```csharp
public CellArea[] GetPrintingPageBreaks(ImageOrPrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | ImageOrPrintOptions | Las opciones de impresión |

### Valor de retorno

Las áreas de saltos de página automáticos.

### Observaciones

Cada área de celda representa una hoja.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPrintingPageBreaksWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para crear saltos de página
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Row {i+1}");
            }

            // Establecer el área de impresión y la configuración de página
            worksheet.PageSetup.PrintArea = "A1:A100";
            worksheet.PageSetup.FitToPagesTall = 1;
            worksheet.PageSetup.FitToPagesWide = 1;

            // Obtener saltos de página con ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            CellArea[] pageBreaks = worksheet.GetPrintingPageBreaks(options);

            // Mostrar la información del primer salto de página
            Console.WriteLine($"First page break ends at row: {pageBreaks[0].EndRow}");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


