---
title: SheetRender Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 100
url: /de/python-net/aspose.cells.rendering/sheetrender/
is_root: false
---
##  SheetRender Klasse
Stellt ein Arbeitsblatt dar, das ein Arbeitsblatt in verschiedene Bilder wie (BMP, PNG, JPEG, TIFF..) rendern kann.
Der Konstruktor dieser Klasse muss nach der Änderung von pagesetup, cell style, verwendet werden.



Der Typ SheetRender macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [SheetRender(worksheet, options)](/cells/de/python-net/aspose.cells.rendering/sheetrender/__init__/#Worksheet-ImageOrPrintOptions) | das Konstrukt von SheetRender, benötigen Arbeitsblatt und ImageOrPrintOptions als Parameter|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [page_count](/cells/de/python-net/aspose.cells.rendering/sheetrender/page_count) | Ruft die Gesamtseitenanzahl des aktuellen Arbeitsblatts ab.|
| [page_scale](/cells/de/python-net/aspose.cells.rendering/sheetrender/page_scale) | Ruft den berechneten Seitenmaßstab des Blatts ab.<br/> Gibt die eingestellte Skala zurück, wenn [PageSetup.zoom](/cells/de/python-net/aspose.cells/pagesetup#zoom) eingestellt ist.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [to_image(page_index, file_name)](/cells/de/python-net/aspose.cells.rendering/sheetrender/to_image/#int-str) | Bestimmte Seiten in eine Datei rendern.|
| [to_image(page_index, stream)](/cells/de/python-net/aspose.cells.rendering/sheetrender/to_image/#int-io.RawIOBase) | Rendern Sie bestimmte Seiten in einen Stream.|
| [to_tiff(stream)](/cells/de/python-net/aspose.cells.rendering/sheetrender/to_tiff/#io.RawIOBase) | Rendern Sie das gesamte Arbeitsblatt als Tiff-Bild zum Streamen.|
| [to_tiff(filename)](/cells/de/python-net/aspose.cells.rendering/sheetrender/to_tiff/#str) | Rendern Sie das gesamte Arbeitsblatt als Tiff-Bild in eine Datei.|
| [to_printer(printer_name)](/cells/de/python-net/aspose.cells.rendering/sheetrender/to_printer/#str) | Arbeitsblatt auf Drucker übertragen|
| [to_printer(printer_name, job_name)](/cells/de/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-str) | Arbeitsblatt auf Drucker übertragen|
| [to_printer(printer_settings)](/cells/de/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Arbeitsblatt auf Drucker übertragen|
| [to_printer(printer_settings, job_name)](/cells/de/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Arbeitsblatt auf Drucker übertragen|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/de/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-int-int) | Arbeitsblatt auf Drucker übertragen|
| [get_page_size_inch(page_index)](/cells/de/python-net/aspose.cells.rendering/sheetrender/get_page_size_inch/#int) |Holen Sie sich die Seitengröße in Zoll des Ausgabebildes.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/de/python-net/aspose.cells.rendering/sheetrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Der Client kann die Seiteneinstellung des Druckers beim Drucken jeder Seite mit dieser Funktion steuern.|



###  Siehe auch
* Modul [aspose.cells.rendering](..)
