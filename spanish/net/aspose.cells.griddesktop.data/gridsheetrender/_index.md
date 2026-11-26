---
title: "Clase GridSheetRender"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridDesktop.Data.GridSheetRender. Representa una representación de hoja de cálculo que puede renderizar la hoja a varias imágenes como BMP, PNG, JPEG, TIFF... El constructor de esta clase debe usarse después de modificar el estilo de celda de la configuración de página"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridsheetrender/
---
## GridSheetRender class

Representa una renderización de hoja de cálculo que puede renderizar la hoja a varias imágenes como (BMP, PNG, JPEG, TIFF...). El constructor de esta clase debe usarse después de modificar la configuración de página y el estilo de celda.

```csharp
public class GridSheetRender
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | la construcción de SheetRender, necesita la hoja de cálculo y ImageOrPrintOptions como parámetros |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | Obtiene el recuento total de páginas de la hoja de cálculo actual. |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | Obtiene la escala de página calculada de la hoja. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | Obtener el tamaño de página en pulgadas de la imagen de salida. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | Renderizar una página específica a un objeto Bitmap. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | Renderizar una página específica a un flujo. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | Renderizar una página específica a un archivo. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Renderizar una página determinada a un Graphics |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Renderizar una página determinada a un Graphics |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | Renderizar la hoja de cálculo a la impresora |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | Renderizar la hoja de cálculo a la impresora |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Renderizar la hoja de cálculo a la impresora |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | Renderizar la hoja de cálculo a la impresora |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | Renderizar toda la hoja de cálculo como imagen Tiff a un flujo. |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | Renderizar toda la hoja de cálculo como imagen Tiff a un archivo. |

### Ver también

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


