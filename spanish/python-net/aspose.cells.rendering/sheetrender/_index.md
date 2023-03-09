---
title: SheetRender clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 100
url: /es/python-net/aspose.cells.rendering/sheetrender/
is_root: false
---
##  SheetRender clase
Representa un procesamiento de hoja de trabajo que puede representar la hoja de trabajo en varias imágenes como (BMP, PNG, JPEG, TIFF...)
El constructor de esta clase debe usarse después de la modificación de la configuración de página, estilo de celda.



El tipo SheetRender expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [SheetRender(worksheet, options)](/cells/es/python-net/aspose.cells.rendering/sheetrender/__init__/#Worksheet-ImageOrPrintOptions) | la construcción de SheetRender, necesita hoja de trabajo e ImageOrPrintOptions como parámetros|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [page_count](/cells/es/python-net/aspose.cells.rendering/sheetrender/page_count) | Obtiene el recuento total de páginas de la hoja de cálculo actual.|
| [page_scale](/cells/es/python-net/aspose.cells.rendering/sheetrender/page_scale) | Obtiene la escala de página calculada de la hoja.<br/> Devuelve la escala establecida si se establece [PageSetup.zoom](/cells/es/python-net/aspose.cells/pagesetup#zoom).|


###  Métodos
| Método| Descripción|
| :- | :- |
| [to_image(page_index, file_name)](/cells/es/python-net/aspose.cells.rendering/sheetrender/to_image/#int-str) | Renderizar ciertas páginas a un archivo.|
| [to_image(page_index, stream)](/cells/es/python-net/aspose.cells.rendering/sheetrender/to_image/#int-io.RawIOBase) | Renderizar ciertas páginas a una secuencia.|
| [to_tiff(stream)](/cells/es/python-net/aspose.cells.rendering/sheetrender/to_tiff/#io.RawIOBase) | Renderice toda la hoja de trabajo como imagen Tiff para transmitir.|
| [to_tiff(filename)](/cells/es/python-net/aspose.cells.rendering/sheetrender/to_tiff/#str) | Renderice toda la hoja de trabajo como imagen Tiff en un archivo.|
| [to_printer(printer_name)](/cells/es/python-net/aspose.cells.rendering/sheetrender/to_printer/#str) | Renderizar la hoja de trabajo a la impresora|
| [to_printer(printer_name, job_name)](/cells/es/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-str) | Renderizar la hoja de trabajo a la impresora|
| [to_printer(printer_settings)](/cells/es/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Renderizar la hoja de trabajo a la impresora|
| [to_printer(printer_settings, job_name)](/cells/es/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Renderizar la hoja de trabajo a la impresora|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/es/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-int-int) | Renderizar la hoja de trabajo a la impresora|
| [get_page_size_inch(page_index)](/cells/es/python-net/aspose.cells.rendering/sheetrender/get_page_size_inch/#int) |Obtenga el tamaño de página en pulgadas de la imagen de salida.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/es/python-net/aspose.cells.rendering/sheetrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | El cliente puede controlar la configuración de la página de la impresora cuando imprima cada página usando esta función.|



###  Ver también
* módulo [aspose.cells.rendering](..)
