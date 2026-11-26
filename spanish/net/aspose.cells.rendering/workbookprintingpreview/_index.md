---
title: "Clase WorkbookPrintingPreview"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.WorkbookPrintingPreview. Vista previa de impresión del libro de trabajo"
type: docs
url: /es/net/aspose.cells.rendering/workbookprintingpreview/
---
## WorkbookPrintingPreview class

Vista previa de impresión del libro de trabajo.

```csharp
public class WorkbookPrintingPreview
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WorkbookPrintingPreview](workbookprintingpreview/)(Workbook, ImageOrPrintOptions) | La construcción de WorkbookPrintingPreview |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/) { get; } | Evaluar el recuento total de páginas de este libro de trabajo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookPrintingPreviewDemo
    {
        public static void WorkbookPrintingPreviewExample()
        {
            // Cargue un libro de trabajo existente
            Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");

            // Cree una instancia de ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Crear una instancia de WorkbookPrintingPreview
            WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);

            // Evaluar el recuento total de páginas del libro de trabajo
            int pageCount = workbookPrintingPreview.EvaluatedPageCount;

            // Imprimir el recuento de páginas evaluado
            Console.WriteLine("Total Page Count: " + pageCount);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


