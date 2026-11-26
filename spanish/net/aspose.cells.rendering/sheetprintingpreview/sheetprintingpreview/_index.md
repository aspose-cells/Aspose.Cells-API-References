---
title: "SheetPrintingPreview.SheetPrintingPreview"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de SheetPrintingPreview. La construcción de SheetPrintingPreview"
type: docs
url: /es/net/aspose.cells.rendering/sheetprintingpreview/sheetprintingpreview/
---
## SheetPrintingPreview constructor

La construcción de SheetPrintingPreview

```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| hoja | Hoja de cálculo | Indicar qué hoja de cálculo se imprimirá. |
| opciones | ImageOrPrintOptions | ImageOrPrintOptions contiene alguna propiedad de salida |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewMethodctorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a la hoja de cálculo
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Crear opciones de imagen/impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Crear vista previa de impresión de hoja
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            // Mostrar el recuento de páginas evaluado
            Console.WriteLine($"Evaluated page count: {preview.EvaluatedPageCount}");
        }
    }
}
```

### Ver también

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


