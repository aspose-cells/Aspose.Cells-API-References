---
title: to_printer Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 50
url: /de/python-net/aspose.cells.rendering/sheetrender/to_printer/
is_root: false
---
##  to_printer(printer_name) {#str}
Arbeitsblatt auf Drucker übertragen



```python
def to_printer(self, printer_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| printer_name | str | der Name des Druckers, zum Beispiel: "Microsoft Office Document Image Writer"|


##  to_printer(printer_settings) {#aspose.pydrawing.printing.PrinterSettings}
Arbeitsblatt auf Drucker übertragen



```python
def to_printer(self, printer_settings):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | die Einstellungen des Druckers, zB PrinterName, Duplex|


##  to_printer(printer_name, job_name) {#str-str}
Arbeitsblatt auf Drucker übertragen



```python
def to_printer(self, printer_name, job_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| printer_name | str | der Name des Druckers, zum Beispiel: "Microsoft Office Document Image Writer"|
| job_name | str | Legen Sie den Namen des Druckauftrags fest|


##  to_printer(printer_settings, job_name) {#aspose.pydrawing.printing.PrinterSettings-str}
Arbeitsblatt auf Drucker übertragen



```python
def to_printer(self, printer_settings, job_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | die Einstellungen des Druckers, zB PrinterName, Duplex|
| job_name | str | Legen Sie den Namen des Druckauftrags fest|


##  to_printer(printer_name, print_page_index, print_page_count) {#str-int-int}
Arbeitsblatt auf Drucker übertragen



```python
def to_printer(self, printer_name, print_page_index, print_page_count):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| printer_name | str | der Name des Druckers, zum Beispiel: "Microsoft Office Document Image Writer"|
| print_page_index | int | Der 0-basierte Index der ersten zu druckenden Seite muss im Bereich [0, SheetRender.PageCount-1] liegen.|
| print_page_count | int | die Anzahl der zu druckenden Seiten, muss größer als Null sein|
###  Bemerkungen

HINWEIS: Diese Methode ist jetzt veraltet.
Verwenden Sie stattdessen ToPrinter(string PrinterName) und ImageOrPrintOptions.PageIndex, PageCount, um die erste Seite und die Anzahl der zu druckenden Seiten festzulegen.
 Diese Property wird 12 Monate später seit Dezember 2021 entfernt.
Aspose entschuldigt sich für etwaige Unannehmlichkeiten.


###  Siehe auch
* Modul [aspose.cells.rendering](../../)
* Klasse [SheetRender](/cells/de/python-net/aspose.cells.rendering/sheetrender)
