---
title: "WorkbookPrintingPreview.WorkbookPrintingPreview"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de WorkbookPrintingPreview. La construcción de WorkbookPrintingPreview"
type: docs
url: /es/net/aspose.cells.rendering/workbookprintingpreview/workbookprintingpreview/
---
## WorkbookPrintingPreview constructor

La construcción de WorkbookPrintingPreview

```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| libro de trabajo | Libro de trabajo | Indique cuál libro de trabajo se debe imprimir. |
| opciones | ImageOrPrintOptions | ImageOrPrintOptions contiene alguna propiedad de salida |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewMethodCtorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Printing Preview");
            
            // Establezca opciones de impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Cree una vista previa de impresión con el libro de trabajo y opciones
            WorkbookPrintingPreview preview = new WorkbookPrintingPreview(workbook, options);
            
            // Muestre el recuento de páginas
            Console.WriteLine("Total pages: " + preview.EvaluatedPageCount);
        }
    }
}
```

### Ver también

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


