---
title: "Clase SheetPrintingPreview"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.SheetPrintingPreview. Vista previa de impresión de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.rendering/sheetprintingpreview/
---
## SheetPrintingPreview class

Vista previa de impresión de la hoja de cálculo.

```csharp
public class SheetPrintingPreview
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SheetPrintingPreview](sheetprintingpreview/)(Worksheet, ImageOrPrintOptions) | La construcción de SheetPrintingPreview |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/) { get; } | Evalúe el recuento total de páginas de esta hoja de cálculo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetPrintingPreviewDemo
    {
        public static void SheetPrintingPreviewExample()
        {
            // Cargue un libro de trabajo existente
            Workbook workbook = new Workbook("SheetPrintingPreviewDemo_original.xlsx");

            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree una instancia de ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Cree una instancia de SheetPrintingPreview
            SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);

            // Evalúe e imprima el recuento total de páginas de la hoja de cálculo
            Console.WriteLine("Total Page Count: " + sheetPrintingPreview.EvaluatedPageCount);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


