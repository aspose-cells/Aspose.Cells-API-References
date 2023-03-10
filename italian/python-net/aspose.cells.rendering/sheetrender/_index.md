---
title: classe SheetRender
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 100
url: /it/python-net/aspose.cells.rendering/sheetrender/
is_root: false
---
##  classe SheetRender
Rappresenta un rendering del foglio di lavoro che può eseguire il rendering del foglio di lavoro in varie immagini come (BMP, PNG, JPEG, TIFF..)
Il costruttore di questa classe, deve essere utilizzato dopo la modifica di pagesetup, cell style.



Il tipo SheetRender espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [SheetRender(worksheet, options)](/cells/it/python-net/aspose.cells.rendering/sheetrender/__init__/#Worksheet-ImageOrPrintOptions) | il costrutto di SheetRender, richiede foglio di lavoro e ImageOrPrintOptions come parametri|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [page_count](/cells/it/python-net/aspose.cells.rendering/sheetrender/page_count) | Ottiene il conteggio totale delle pagine del foglio di lavoro corrente.|
| [page_scale](/cells/it/python-net/aspose.cells.rendering/sheetrender/page_scale) | Ottiene la scala di pagina calcolata del foglio.<br/> Restituisce la scala impostata se è impostato [PageSetup.zoom](/cells/it/python-net/aspose.cells/pagesetup#zoom). In caso contrario, restituisce la scala calcolata secondo [PageSetup.fit_to_pages_wide](/cells/it/python-net/aspose.cells/pagesetup#fit_to_pages_wide) e [PageSetup.fit_to_pages_tall](/cells/it/python-net/aspose.cells/pagesetup#fit_to_pages_tall).|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [to_image(page_index, file_name)](/cells/it/python-net/aspose.cells.rendering/sheetrender/to_image/#int-str) | Renderizza determinate pagine in un file.|
| [to_image(page_index, stream)](/cells/it/python-net/aspose.cells.rendering/sheetrender/to_image/#int-io.RawIOBase) | Renderizza determinate pagine in un flusso.|
| [to_tiff(stream)](/cells/it/python-net/aspose.cells.rendering/sheetrender/to_tiff/#io.RawIOBase) | Renderizza l'intero foglio di lavoro come immagine Tiff per lo streaming.|
| [to_tiff(filename)](/cells/it/python-net/aspose.cells.rendering/sheetrender/to_tiff/#str) | Renderizza l'intero foglio di lavoro come immagine Tiff in un file.|
| [to_printer(printer_name)](/cells/it/python-net/aspose.cells.rendering/sheetrender/to_printer/#str) | Renderizza il foglio di lavoro alla stampante|
| [to_printer(printer_name, job_name)](/cells/it/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-str) | Renderizza il foglio di lavoro alla stampante|
| [to_printer(printer_settings)](/cells/it/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Renderizza il foglio di lavoro alla stampante|
| [to_printer(printer_settings, job_name)](/cells/it/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Renderizza il foglio di lavoro alla stampante|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/it/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-int-int) | Renderizza il foglio di lavoro alla stampante|
| [get_page_size_inch(page_index)](/cells/it/python-net/aspose.cells.rendering/sheetrender/get_page_size_inch/#int) |Ottieni le dimensioni della pagina in pollici dell'immagine di output.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/it/python-net/aspose.cells.rendering/sheetrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Il client può controllare l'impostazione della pagina della stampante quando stampa ciascuna pagina utilizzando questa funzione.|



###  Guarda anche
* modulo [aspose.cells.rendering](..)
