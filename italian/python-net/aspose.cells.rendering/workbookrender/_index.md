---
title: classe WorkbookRender
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 130
url: /it/python-net/aspose.cells.rendering/workbookrender/
is_root: false
---
##  classe WorkbookRender
 Rappresenta un rendering della cartella di lavoro.
Il costruttore di questa classe, deve essere utilizzato dopo la modifica di pagesetup, cell style.



Il tipo WorkbookRender espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [WorkbookRender(workbook, options)](/cells/it/python-net/aspose.cells.rendering/workbookrender/__init__/#Workbook-ImageOrPrintOptions) | Il costrutto di WorkbookRender|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [page_count](/cells/it/python-net/aspose.cells.rendering/workbookrender/page_count) | Ottiene il conteggio totale delle pagine della cartella di lavoro.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [to_image(stream)](/cells/it/python-net/aspose.cells.rendering/workbookrender/to_image/#io.RawIOBase) | Renderizza l'intera cartella di lavoro come immagine Tiff per lo streaming.|
| [to_image(filename)](/cells/it/python-net/aspose.cells.rendering/workbookrender/to_image/#str) | Renderizza l'intera cartella di lavoro come immagine Tiff in un file.|
| [to_image(page_index, file_name)](/cells/it/python-net/aspose.cells.rendering/workbookrender/to_image/#int-str) | Renderizza determinate pagine in un file.|
| [to_image(page_index, stream)](/cells/it/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.RawIOBase) | Renderizza determinate pagine in un flusso.|
| [to_printer(printer_name)](/cells/it/python-net/aspose.cells.rendering/workbookrender/to_printer/#str) | Renderizza la cartella di lavoro sulla stampante|
| [to_printer(printer_name, job_name)](/cells/it/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-str) | Renderizza la cartella di lavoro sulla stampante|
| [to_printer(printer_settings)](/cells/it/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Renderizza la cartella di lavoro sulla stampante|
| [to_printer(printer_settings, job_name)](/cells/it/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Renderizza la cartella di lavoro sulla stampante|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/it/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-int-int) | Renderizza la cartella di lavoro sulla stampante|
| [get_page_size_inch(page_index)](/cells/it/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) |Ottieni le dimensioni della pagina in pollici dell'immagine di output.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/it/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Il client può controllare l'impostazione della pagina della stampante quando stampa ciascuna pagina utilizzando questa funzione.|



###  Osservazioni



###  Guarda anche
* modulo [aspose.cells.rendering](..)
