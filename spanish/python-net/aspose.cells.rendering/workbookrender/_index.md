---
title: WorkbookRender clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 130
url: /es/python-net/aspose.cells.rendering/workbookrender/
is_root: false
---
##  WorkbookRender clase
 Representa una representación de libro de trabajo.
El constructor de esta clase debe usarse después de la modificación de la configuración de página, estilo de celda.



El tipo WorkbookRender expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [WorkbookRender(workbook, options)](/cells/es/python-net/aspose.cells.rendering/workbookrender/__init__/#Workbook-ImageOrPrintOptions) | La construcción de WorkbookRender|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [page_count](/cells/es/python-net/aspose.cells.rendering/workbookrender/page_count) | Obtiene el número total de páginas de los libros de trabajo.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [to_image(stream)](/cells/es/python-net/aspose.cells.rendering/workbookrender/to_image/#io.RawIOBase) | Renderice todo el libro de trabajo como imagen Tiff para transmitir.|
| [to_image(filename)](/cells/es/python-net/aspose.cells.rendering/workbookrender/to_image/#str) | Renderice todo el libro de trabajo como imagen Tiff en un archivo.|
| [to_image(page_index, file_name)](/cells/es/python-net/aspose.cells.rendering/workbookrender/to_image/#int-str) | Renderizar ciertas páginas a un archivo.|
| [to_image(page_index, stream)](/cells/es/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.RawIOBase) | Renderizar ciertas páginas a una secuencia.|
| [to_printer(printer_name)](/cells/es/python-net/aspose.cells.rendering/workbookrender/to_printer/#str) | Renderizar el libro de trabajo a la impresora|
| [to_printer(printer_name, job_name)](/cells/es/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-str) | Renderizar el libro de trabajo a la impresora|
| [to_printer(printer_settings)](/cells/es/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Renderizar el libro de trabajo a la impresora|
| [to_printer(printer_settings, job_name)](/cells/es/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Renderizar el libro de trabajo a la impresora|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/es/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-int-int) | Renderizar el libro de trabajo a la impresora|
| [get_page_size_inch(page_index)](/cells/es/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) |Obtenga el tamaño de página en pulgadas de la imagen de salida.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/es/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | El cliente puede controlar la configuración de la página de la impresora cuando imprima cada página usando esta función.|



###  Observaciones



###  Ver también
* módulo [aspose.cells.rendering](..)
