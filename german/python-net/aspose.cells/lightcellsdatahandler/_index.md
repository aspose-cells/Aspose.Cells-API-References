---
title: LightCellsDataHandler Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 990
url: /de/python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---
##  LightCellsDataHandler Klasse
Repräsentiert den Datenhandler für Zellen zum Lesen großer Tabellenkalkulationsdateien im einfachen Modus.



Der Typ LightCellsDataHandler macht die folgenden Member verfügbar:

###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [start_sheet(sheet)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) | Beginnt mit der Verarbeitung eines Arbeitsblatts.|
| [start_row(row_index)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) | Bereitet die Verarbeitung einer Zeile vor.|
| [process_row(row)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) | Beginnt mit der Verarbeitung einer Zeile.|
| [start_cell(column_index)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | Bereitet die Verarbeitung einer Zelle vor.|
| [process_cell(cell)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) | Beginnt mit der Verarbeitung einer Zelle.|



###  Bemerkungen

Beim Lesen einer Arbeitsmappe in diesem Modus wird [LightCellsDataHandler.start_sheet(sheet)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/start_sheet) überprüft, wenn jedes Arbeitsblatt in der Arbeitsmappe gelesen wird.
Wenn für ein Blatt [LightCellsDataHandler.start_sheet(sheet)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/start_sheet) wahr ist, werden alle Daten und Eigenschaften von Zeilen/Zellen dieses Blattes überprüft
und von der Implementierung dieser Schnittstelle verarbeitet.Für jede Zeile wird [LightCellsDataHandler.start_row(row_index)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/start_row) aufgerufen, um zu prüfen, ob sie verarbeitetwerden muss.
Wenn eine Zeile verarbeitet werden muss, werden die Eigenschaften dieser Zeile zuerst gelesen und der Benutzer kann bis [LightCellsDataHandler.process_row(row)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/process_row) auf seine Eigenschaften zugreifen.
Wenn auch Zeilenzellen verarbeitet werden müssen, sollte [LightCellsDataHandler.process_row(row)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/process_row) wahr zurückgeben, und dann wird [LightCellsDataHandler.start_cell(column_index)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/start_cell) wahr sein
für jede vorhandene Zelle in dieser Zeile aufgerufen, um zu prüfen, ob eine Zelle verarbeitet werden muss.
dann wird [LightCellsDataHandler.process_cell(cell)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/process_cell) aufgerufen, um die Zelle durch die Implementierung dieser Schnittstelle zu verarbeiten.

###  Siehe auch
* Modul [aspose.cells](..)
