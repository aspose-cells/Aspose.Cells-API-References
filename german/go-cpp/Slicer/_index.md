---
title: "Slicer Klasse"
linktitle: "Slicer"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Slicer-Klasse. Kapselt das Objekt, das den slicer in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/slicer/
---

## Slicer class

Zusammenfassende Beschreibung der Slicer-Ansicht

```go

type Slicer struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetSortOrderType](./getsortordertype/) | Gibt den Typ der Sortierelemente an. |
| [SetSortOrderType](./setsortordertype/) | Gibt den Typ der Sortierelemente an. |
| [GetShowMissing](./getshowmissing/) | Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen. |
| [SetShowMissing](./setshowmissing/) | Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen. |
| [GetShowTypeOfItemsWithNoData](./getshowtypeofitemswithnodata/) | Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen. |
| [SetShowTypeOfItemsWithNoData](./setshowtypeofitemswithnodata/) | Gibt an, ob Elemente, die aus der Datenquelle gelöscht wurden, angezeigt werden sollen. |
| [GetShowAllItems](./getshowallitems/) | Gibt an, ob alle Elemente angezeigt werden sollen, selbst wenn keine Daten vorhanden sind oder sie gelöscht wurden. Standardwert ist true; |
| [SetShowAllItems](./setshowallitems/) | Gibt an, ob alle Elemente angezeigt werden sollen, selbst wenn keine Daten vorhanden sind oder sie gelöscht wurden. Standardwert ist true; |
| [AddPivotConnection](./addpivotconnection/) | Fügt eine PivotTable-Verbindung hinzu. |
| [RemovePivotConnection](./removepivotconnection/) | Entfernt die PivotTable-Verbindung. |
| [GetLockedPosition](./getlockedposition/) | Gibt an, ob der angegebene Slicer über die Benutzeroberfläche verschoben oder in der Größe geändert werden kann. |
| [SetLockedPosition](./setlockedposition/) | Gibt an, ob der angegebene Slicer über die Benutzeroberfläche verschoben oder in der Größe geändert werden kann. |
| [Refresh](./refresh/) | Aktualisieren der Elemente des Slicers aus den zugehörigen Pivot-Tabellen. |
| [GetShape](./getshape/) | Gibt das Shape-Objekt zurück, das dem angegebenen Slicer zugeordnet ist. Nur lesbar. |
| [GetSlicerCache](./getslicercache/) | Gibt das SlicerCache-Objekt zurück, das dem Slicer zugeordnet ist. Nur lesbar. |
| [GetWorksheet](./getworksheet/) | Gibt das Worksheet-Objekt zurück, das diesen Slicer enthält. Nur lesbar. |
| [GetStyleType](./getstyletype/) | Geben Sie den Typ des integrierten Slicer-Stils an. Der Standardtyp ist SlicerStyleLight1. |
| [SetStyleType](./setstyletype/) | Geben Sie den Typ des integrierten Slicer-Stils an. Der Standardtyp ist SlicerStyleLight1. |
| [GetName](./getname/) | Gibt den Namen des angegebenen Slicers zurück oder legt ihn fest |
| [SetName](./setname/) | Gibt den Namen des angegebenen Slicers zurück oder legt ihn fest |
| [GetCaption](./getcaption/) | Gibt die Beschriftung des angegebenen Slicers zurück oder legt sie fest. |
| [SetCaption](./setcaption/) | Gibt die Beschriftung des angegebenen Slicers zurück oder legt sie fest. |
| [GetFirstItemIndex](./getfirstitemindex/) | Gibt den nullbasierten Index des ersten Slicer-Elements an. |
| [SetFirstItemIndex](./setfirstitemindex/) | Gibt den nullbasierten Index des ersten Slicer-Elements an. |
|[SelectItems](./selectitems/) |  | 
| [UnselectItems](./unselectitems/) | Ausgewählte Filterbeschriftungen entfernen. |
| [ClearFilter](./clearfilter/) | Filter entfernen |
| [GetShowCaption](./getshowcaption/) | Gibt an, ob die Kopfzeile des Slicers sichtbar ist. Der Standardwert ist true |
| [SetShowCaption](./setshowcaption/) | Gibt an, ob die Kopfzeile des Slicers sichtbar ist. Der Standardwert ist true |
| [GetNumberOfColumns](./getnumberofcolumns/) | Gibt die Anzahl der Spalten im Slicer zurück oder legt sie fest. Der Standardwert ist 1. |
| [SetNumberOfColumns](./setnumberofcolumns/) | Gibt die Anzahl der Spalten im Slicer zurück oder legt sie fest. Der Standardwert ist 1. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Gibt die Breite jeder Spalte im Slicer zurück oder legt sie fest, in Pixel. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Gibt die Breite jeder Spalte im Slicer zurück oder legt sie fest, in Pixel. |
| [GetColumnWidth](./getcolumnwidth/) | Gibt die Breite jeder Spalte im Slicer zurück oder legt sie fest, in Punkt. |
| [SetColumnWidth](./setcolumnwidth/) | Gibt die Breite jeder Spalte im Slicer zurück oder legt sie fest, in Punkt. |
| [GetRowHeightPixel](./getrowheightpixel/) | Gibt die Höhe jeder Zeile im angegebenen Slicer zurück oder legt sie fest, in Pixel. |
| [SetRowHeightPixel](./setrowheightpixel/) | Gibt die Höhe jeder Zeile im angegebenen Slicer zurück oder legt sie fest, in Pixel. |
| [GetRowHeight](./getrowheight/) | Gibt die Höhe jeder Zeile im angegebenen Slicer zurück oder legt sie fest, in Punkt. |
| [SetRowHeight](./setrowheight/) | Gibt die Höhe jeder Zeile im angegebenen Slicer zurück oder legt sie fest, in Punkt. |
