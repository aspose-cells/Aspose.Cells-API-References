---
title: to_printer método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells.rendering/sheetrender/to_printer/
is_root: false
---
##  to_printer(printer_name) {#str}
Renderizar la hoja de trabajo a la impresora



```python
def to_printer(self, printer_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| printer_name | str | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer"|


##  to_printer(printer_settings) {#aspose.pydrawing.printing.PrinterSettings}
Renderizar la hoja de trabajo a la impresora



```python
def to_printer(self, printer_settings):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | la configuración de la impresora, por ejemplo, PrinterName, Duplex|


##  to_printer(printer_name, job_name) {#str-str}
Renderizar la hoja de trabajo a la impresora



```python
def to_printer(self, printer_name, job_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| printer_name | str | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer"|
| job_name | str | establecer el nombre del trabajo de impresión|


##  to_printer(printer_settings, job_name) {#aspose.pydrawing.printing.PrinterSettings-str}
Renderizar la hoja de trabajo a la impresora



```python
def to_printer(self, printer_settings, job_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | la configuración de la impresora, por ejemplo, PrinterName, Duplex|
| job_name | str | establecer el nombre del trabajo de impresión|


##  to_printer(printer_name, print_page_index, print_page_count) {#str-int-int}
Renderizar la hoja de trabajo a la impresora



```python
def to_printer(self, printer_name, print_page_index, print_page_count):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| printer_name | str | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer"|
| print_page_index | int |el índice basado en 0 de la primera página a imprimir, debe estar en el rango [0, SheetRender.PageCount-1]|
| print_page_count | int | el número de páginas a imprimir, debe ser mayor que cero|
###  Observaciones

NOTA: Este método ahora está obsoleto.
En su lugar, utilice ToPrinter(string PrinterName) e ImageOrPrintOptions.PageIndex, PageCount para establecer la primera página y el número de páginas a imprimir.
 Esta propiedad se eliminará 12 meses después desde diciembre de 2021.
Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.


###  Ver también
* módulo [aspose.cells.rendering](../../)
* clase [SheetRender](/cells/es/python-net/aspose.cells.rendering/sheetrender)
