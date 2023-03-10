---
title: metodo to_printer
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 50
url: /it/python-net/aspose.cells.rendering/sheetrender/to_printer/
is_root: false
---
##  to_printer(printer_name) {#str}
Renderizza il foglio di lavoro alla stampante



```python
def to_printer(self, printer_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| printer_name | str | il nome della stampante, ad esempio: "Microsoft Office Document Image Writer"|


##  to_printer(printer_settings) {#aspose.pydrawing.printing.PrinterSettings}
Renderizza il foglio di lavoro alla stampante



```python
def to_printer(self, printer_settings):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | le impostazioni della stampante, ad esempio PrinterName, Duplex|


##  to_printer(printer_name, job_name) {#str-str}
Renderizza il foglio di lavoro alla stampante



```python
def to_printer(self, printer_name, job_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| printer_name | str | il nome della stampante, ad esempio: "Microsoft Office Document Image Writer"|
| job_name | str | impostare il nome del lavoro di stampa|


##  to_printer(printer_settings, job_name) {#aspose.pydrawing.printing.PrinterSettings-str}
Renderizza il foglio di lavoro alla stampante



```python
def to_printer(self, printer_settings, job_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | le impostazioni della stampante, ad esempio PrinterName, Duplex|
| job_name | str | impostare il nome del lavoro di stampa|


##  to_printer(printer_name, print_page_index, print_page_count) {#str-int-int}
Renderizza il foglio di lavoro alla stampante



```python
def to_printer(self, printer_name, print_page_index, print_page_count):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| printer_name | str | il nome della stampante, ad esempio: "Microsoft Office Document Image Writer"|
| print_page_index | int | l'indice in base 0 della prima pagina da stampare, deve essere compreso nell'intervallo [0, SheetRender.PageCount-1]|
| print_page_count | int | il numero di pagine da stampare, deve essere maggiore di zero|
###  Osservazioni

NOTA: questo metodo è ora obsoleto.
Utilizzare invece ToPrinter(string PrinterName) e ImageOrPrintOptions.PageIndex, PageCount per impostare la prima pagina e il numero di pagine da stampare.
 Questa proprietà verrà rimossa 12 mesi dopo da dicembre 2021.
Aspose si scusa per gli eventuali disagi causati.


###  Guarda anche
* modulo [aspose.cells.rendering](../../)
* classe [SheetRender](/cells/it/python-net/aspose.cells.rendering/sheetrender)
