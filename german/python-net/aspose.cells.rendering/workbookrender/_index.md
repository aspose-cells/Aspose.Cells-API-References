---
title: WorkbookRender Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 130
url: /de/python-net/aspose.cells.rendering/workbookrender/
is_root: false
---
##  WorkbookRender Klasse
 Stellt ein Arbeitsmappen-Rendering dar.
Der Konstruktor dieser Klasse muss nach der Änderung von pagesetup, cell style, verwendet werden.



Der Typ WorkbookRender macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [WorkbookRender(workbook, options)](/cells/de/python-net/aspose.cells.rendering/workbookrender/__init__/#Workbook-ImageOrPrintOptions) | Das Konstrukt von WorkbookRender|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [page_count](/cells/de/python-net/aspose.cells.rendering/workbookrender/page_count) | Ruft die Gesamtseitenanzahl von Arbeitsmappen ab.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [to_image(stream)](/cells/de/python-net/aspose.cells.rendering/workbookrender/to_image/#io.RawIOBase) | Rendern Sie die gesamte Arbeitsmappe als Tiff-Bild zum Streamen.|
| [to_image(filename)](/cells/de/python-net/aspose.cells.rendering/workbookrender/to_image/#str) | Rendern Sie die gesamte Arbeitsmappe als Tiff-Bild in eine Datei.|
| [to_image(page_index, file_name)](/cells/de/python-net/aspose.cells.rendering/workbookrender/to_image/#int-str) | Bestimmte Seiten in eine Datei rendern.|
| [to_image(page_index, stream)](/cells/de/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.RawIOBase) | Rendern Sie bestimmte Seiten in einen Stream.|
| [to_printer(printer_name)](/cells/de/python-net/aspose.cells.rendering/workbookrender/to_printer/#str) | Arbeitsmappe auf Drucker übertragen|
| [to_printer(printer_name, job_name)](/cells/de/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-str) | Arbeitsmappe auf Drucker übertragen|
| [to_printer(printer_settings)](/cells/de/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Arbeitsmappe auf Drucker übertragen|
| [to_printer(printer_settings, job_name)](/cells/de/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Arbeitsmappe auf Drucker übertragen|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/de/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-int-int) | Arbeitsmappe auf Drucker übertragen|
| [get_page_size_inch(page_index)](/cells/de/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) |Holen Sie sich die Seitengröße in Zoll des Ausgabebildes.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/de/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Der Client kann die Seiteneinstellung des Druckers beim Drucken jeder Seite mit dieser Funktion steuern.|



###  Bemerkungen



###  Siehe auch
* Modul [aspose.cells.rendering](..)
