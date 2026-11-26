---
title: "Clase SheetRender"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.SheetRender. Representa una representación de hoja de cálculo que puede renderizar la hoja a varias imágenes como BMP, PNG, JPEG, TIFF. El constructor de esta clase debe usarse después de modificar el estilo de celda de la configuración de página."
type: docs
url: /es/net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

Representa una renderización de hoja de cálculo que puede renderizar la hoja a varias imágenes como (BMP, PNG, JPEG, TIFF...). El constructor de esta clase debe usarse después de modificar la configuración de página y el estilo de celda.

```csharp
public class SheetRender
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SheetRender](sheetrender/)(Worksheet, ImageOrPrintOptions) | la construcción de SheetRender, necesita la hoja de cálculo y ImageOrPrintOptions como parámetros |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount/) { get; } | Obtiene el recuento total de páginas de la hoja de cálculo actual. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale/) { get; } | Obtiene la escala de página calculada de la hoja. Devuelve la escala establecida si [`Zoom`](../../aspose.cells/pagesetup/zoom/) está configurado. De lo contrario, devuelve la escala calculada según [`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide/) y [`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall/). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint/)(bool, PrintPageEventArgs) | El cliente puede controlar la configuración de página de la impresora al imprimir cada página usando esta función. |
| [Dispose](../../aspose.cells.rendering/sheetrender/dispose/)() | Libera los recursos creados y usados para el renderizado. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch/)(int) | Obtener el tamaño de página en pulgadas de la imagen de salida. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage)(int) | Renderizar una página específica a un objeto Bitmap. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_3)(int, Stream) | Renderizar una página específica a un flujo. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_4)(int, string) | Renderizar una página específica a un archivo. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Renderizar una página determinada a un Graphics |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Renderizar una página determinada a un Graphics |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter)(PrinterSettings) | Renderizar la hoja de cálculo a la impresora |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_2)(string) | Renderizar la hoja de cálculo a la impresora |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Renderizar la hoja de cálculo a la impresora |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_4)(string, string) | Renderizar la hoja de cálculo a la impresora |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_3)(string, int, int) | (**Obsoleto.**) Renderizar la hoja de cálculo a la impresora |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff)(Stream) | Renderizar toda la hoja de cálculo como imagen Tiff a un flujo. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff_1)(string) | Renderizar toda la hoja de cálculo como imagen Tiff a un archivo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassSheetRenderDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Configurar la configuración de página
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.PrintArea = "1:10";
            pageSetup.SetFitToPages(1, 1);

            // Crear SheetRender y demostrar la funcionalidad principal
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender sr = new SheetRender(sheet, options);
            
            Console.WriteLine($"Number of pages: {sr.PageCount}");
            Console.WriteLine($"Page scale: {sr.PageScale * 100}%");
            
            // Renderizar la primera página a una imagen (demostración)
            sr.ToImage(0, "output_page1.png");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


