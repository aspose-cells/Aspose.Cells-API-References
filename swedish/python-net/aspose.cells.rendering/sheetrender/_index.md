---
title: SheetRender klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 100
url: /sv/python-net/aspose.cells.rendering/sheetrender/
is_root: false
---
##  SheetRender klass
Representerar en kalkylbladsrendering som kan rendera kalkylblad till olika bilder som (BMP, PNG, JPEG, TIFF..)
Konstruktorn för denna klass måste användas efter modifiering av sidinställningar, cellstil.



Typen SheetRender avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [SheetRender(worksheet, options)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/__init__/#Worksheet-ImageOrPrintOptions) | konstruktionen av SheetRender, behöver kalkylblad och ImageOrPrintOptions som parametrar|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [page_count](/cells/sv/python-net/aspose.cells.rendering/sheetrender/page_count) | Hämtar det totala antalet sidor för det aktuella kalkylbladet.|
| [page_scale](/cells/sv/python-net/aspose.cells.rendering/sheetrender/page_scale) | Får beräknad sidskala på arket.<br/> Returnerar den inställda skalan om [PageSetup.zoom](/cells/sv/python-net/aspose.cells/pagesetup#zoom) är inställd.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [to_image(page_index, file_name)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/to_image/#int-str) | Rendera vissa sidor till en fil.|
| [to_image(page_index, stream)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/to_image/#int-io.RawIOBase) | Rendera vissa sidor till en stream.|
| [to_tiff(stream)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/to_tiff/#io.RawIOBase) | Gör hela kalkylbladet som Tiff-bild för att streama.|
| [to_tiff(filename)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/to_tiff/#str) | Gör hela kalkylbladet som Tiff-bild till en fil.|
| [to_printer(printer_name)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/to_printer/#str) | Återge arbetsbladet till skrivaren|
| [to_printer(printer_name, job_name)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-str) | Återge arbetsbladet till skrivaren|
| [to_printer(printer_settings)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Återge arbetsbladet till skrivaren|
| [to_printer(printer_settings, job_name)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Återge arbetsbladet till skrivaren|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-int-int) | Återge arbetsbladet till skrivaren|
| [get_page_size_inch(page_index)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/get_page_size_inch/#int) |Få sidstorlek i tum av utdatabilden.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/sv/python-net/aspose.cells.rendering/sheetrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Klienten kan styra sidinställningarna för skrivaren när du skriver ut varje sida med denna funktion.|



###  Se även
* modul [aspose.cells.rendering](..)
