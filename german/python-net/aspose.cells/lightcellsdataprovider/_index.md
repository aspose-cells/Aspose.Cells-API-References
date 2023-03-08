---
title: LightCellsDataProvider Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1000
url: /de/python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---
##  LightCellsDataProvider Klasse
Stellt den Datenanbieter zum Speichern großer Tabellenkalkulationsdateien im einfachen Modus dar.



Der Typ LightCellsDataProvider macht die folgenden Member verfügbar:

###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [start_sheet(sheet_index)](/cells/de/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | Beginnt mit dem Speichern eines Arbeitsblatts.|
| [next_row()](/cells/de/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | Ruft die nächste zu speichernde Zeile ab.|
| [start_row(row)](/cells/de/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) | Beginnt mit dem Speichern der Daten einer Zeile.|
| [next_cell()](/cells/de/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | Ruft die nächste zu speichernde Zelle ab.|
| [start_cell(cell)](/cells/de/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) | Beginnt mit dem Speichern der Daten einer Zelle.|
| [is_gather_string()](/cells/de/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) |Überprüft, ob der aktuelle Zeichenfolgenwert der Zelle in einem globalen Pool gesammelt werden muss.|



###  Bemerkungen

Beim Speichern einer Arbeitsmappe in diesem Modus wird [LightCellsDataProvider.start_sheet(sheet_index)](/cells/de/python-net/aspose.cells/lightcellsdataprovider/start_sheet) überprüft, wenn jedes Arbeitsblatt in der Arbeitsmappe gespeichert wird.
Wenn für ein Blatt [LightCellsDataProvider.start_sheet(sheet_index)](/cells/de/python-net/aspose.cells/lightcellsdataprovider/start_sheet) wahr ist, werden alle Daten und Eigenschaften von Zeilen/Zellen dieses Blattes gespeichert
wird durch die Implementierung dieser Schnittstelle bereitgestellt. Zunächst wird [LightCellsDataProvider.next_row()](/cells/de/python-net/aspose.cells/lightcellsdataprovider/next_row) aufgerufen, um den nächsten zu speichernden Zeilenindex zu erhalten.
Wenn ein gültiger Zeilenindex zurückgegeben wird (der Zeilenindex muss in aufsteigender Reihenfolge sein, damit die Zeilen gespeichert werden können),
dann wird ein Zeilenobjekt, das diese Zeile darstellt, zur Implementierung bereitgestellt, um seine Eigenschaften bis [LightCellsDataProvider.start_row(row)](/cells/de/python-net/aspose.cells/lightcellsdataprovider/start_row) festzulegen.
Für eine Zeile wird zuerst [LightCellsDataProvider.next_cell()](/cells/de/python-net/aspose.cells/lightcellsdataprovider/next_cell) geprüft. Wenn ein gültiger Spaltenindex zurückgegeben wird (der Spaltenindex muss in aufsteigender Reihenfolge sein, damit alle Zellen einer Zeile gespeichert werden),
dann wird ein Cell-Objekt, das diese Zelle darstellt, zur Implementierung bereitgestellt, um seine Daten und Eigenschaften von [LightCellsDataProvider.start_cell(cell)](/cells/de/python-net/aspose.cells/lightcellsdataprovider/start_cell) festzulegen.
Nachdem die Daten dieser Zelle eingestellt wurden, wird diese Zelle direkt in der generierten Tabellendatei gespeichert und die nächste Zelle wird geprüft und verarbeitet.

###  Siehe auch
* Modul [aspose.cells](..)
