---
title: WorkbookRender klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 130
url: /sv/python-net/aspose.cells.rendering/workbookrender/
is_root: false
---
##  WorkbookRender klass
 Representerar en återgivning av en arbetsbok.
Konstruktorn för denna klass måste användas efter modifiering av sidinställningar, cellstil.



Typen WorkbookRender avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [WorkbookRender(workbook, options)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/__init__/#Workbook-ImageOrPrintOptions) | Konstruktionen av WorkbookRender|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [page_count](/cells/sv/python-net/aspose.cells.rendering/workbookrender/page_count) | Får det totala antalet sidor av arbetsböcker.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [to_image(stream)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/to_image/#io.RawIOBase) | Gör hela arbetsboken som Tiff-bild för att streama.|
| [to_image(filename)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/to_image/#str) | Rendera hela arbetsboken som Tiff-bild till en fil.|
| [to_image(page_index, file_name)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/to_image/#int-str) | Rendera vissa sidor till en fil.|
| [to_image(page_index, stream)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.RawIOBase) | Rendera vissa sidor till en stream.|
| [to_printer(printer_name)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/to_printer/#str) | Gör arbetsboken till skrivaren|
| [to_printer(printer_name, job_name)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-str) | Gör arbetsboken till skrivaren|
| [to_printer(printer_settings)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Gör arbetsboken till skrivaren|
| [to_printer(printer_settings, job_name)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Gör arbetsboken till skrivaren|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-int-int) | Gör arbetsboken till skrivaren|
| [get_page_size_inch(page_index)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) |Få sidstorlek i tum av utdatabilden.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/sv/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Klienten kan styra sidinställningarna för skrivaren när du skriver ut varje sida med denna funktion.|



###  Anmärkningar



###  Se även
* modul [aspose.cells.rendering](..)
