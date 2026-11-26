---
title: "Clase WorkbookRender"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.WorkbookRender. Representa una representación de libro de trabajo. El constructor de esta clase debe usarse después de la modificación del estilo de celda de configuración de página"
type: docs
url: /es/net/aspose.cells.rendering/workbookrender/
---
## WorkbookRender class

Representa una renderización de libro de trabajo. El constructor de esta clase debe usarse después de modificar la configuración de página y el estilo de celda.

```csharp
public class WorkbookRender
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | La construcción de WorkbookRender |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | Obtiene el recuento total de páginas del libro de trabajo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | El cliente puede controlar la configuración de página de la impresora al imprimir cada página usando esta función. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | Libera los recursos creados y usados para el renderizado. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | Obtener el tamaño de página en pulgadas de la imagen de salida. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | Renderizar una página específica a un objeto Bitmap. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | Renderizar todo el libro de trabajo como imagen Tiff a un flujo. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | Renderizar todo el libro de trabajo como imagen Tiff a un archivo. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | Renderizar una página específica a un flujo. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | Renderizar una página específica a un archivo. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | Renderizar libro de trabajo a la impresora |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | Renderizar libro de trabajo a la impresora |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | Renderizar libro de trabajo a la impresora |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | Renderizar libro de trabajo a la impresora |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Obsoleto.**) Renderizar libro de trabajo a la impresora |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassWorkbookRenderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y establecer el tamaño de página
            worksheet.Cells["A1"].PutValue("Workbook Render Demo");
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Crear opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Crear el renderizado del libro de trabajo y obtener el tamaño de página
            WorkbookRender render = new WorkbookRender(workbook, options);
            float[] pageSize = render.GetPageSizeInch(0);
            
            // Genere la salida de los resultados
            Console.WriteLine($"Page Width: {pageSize[0]} inches");
            Console.WriteLine($"Page Height: {pageSize[1]} inches");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


