---
title: "ImportTableOptions Klasse"
linktitle: "ImportTableOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ImportTableOptions Klasse. Kapselt das Objekt, das importtableoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/importtableoptions/
---

## ImportTableOptions class

Stellt die Optionen zum Importieren von Daten in Zellen dar.

```go

type ImportTableOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewImportTableOptions](./newimporttableoptions/) | Erstellt die Standard‑Importoptionen. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetConvertGridStyle](./getconvertgridstyle/) | Gibt an, ob der Stil der Grid‑Ansicht auf Zellen angewendet wird. |
| [SetConvertGridStyle](./setconvertgridstyle/) | Gibt an, ob der Stil der Grid‑Ansicht auf Zellen angewendet wird. |
| [GetConvertNumericData](./getconvertnumericdata/) | Liest oder setzt einen Wert, der angibt, ob der Zeichenkettenwert in einen numerischen oder Datumswert konvertiert werden soll. |
| [SetConvertNumericData](./setconvertnumericdata/) | Liest oder setzt einen Wert, der angibt, ob der Zeichenkettenwert in einen numerischen oder Datumswert konvertiert werden soll. |
| [GetInsertRows](./getinsertrows/) | Gibt an, ob neue Zeilen für das Importieren von Datensätzen hinzugefügt werden sollen. |
| [SetInsertRows](./setinsertrows/) | Gibt an, ob neue Zeilen für das Importieren von Datensätzen hinzugefügt werden sollen. |
| [GetShiftFirstRowDown](./getshiftfirstrowdown/) | Gibt an, ob die erste Zeile beim Einfügen von Zeilen nach unten verschoben wird. |
| [SetShiftFirstRowDown](./setshiftfirstrowdown/) | Gibt an, ob die erste Zeile beim Einfügen von Zeilen nach unten verschoben wird. |
| [IsFieldNameShown](./isfieldnameshown/) | Gibt an, ob Feldnamen importiert werden sollen. |
| [SetIsFieldNameShown](./setisfieldnameshown/) | Gibt an, ob Feldnamen importiert werden sollen. |
| [GetExportCaptionAsFieldName](./getexportcaptionasfieldname/) | Gibt an, ob die Beschriftung als Feldname exportiert wird |
| [SetExportCaptionAsFieldName](./setexportcaptionasfieldname/) | Gibt an, ob die Beschriftung als Feldname exportiert wird |
| [GetDateFormat](./getdateformat/) | Liest oder setzt das Datumsformatzeichenfolge für Zellen mit importierten Datums‑Uhrzeit‑Werten. |
| [SetDateFormat](./setdateformat/) | Liest oder setzt das Datumsformatzeichenfolge für Zellen mit importierten Datums‑Uhrzeit‑Werten. |
| [GetNumberFormats](./getnumberformats/) | Liest oder setzt die Zahlenformate |
| [SetNumberFormats](./setnumberformats/) | Liest oder setzt die Zahlenformate |
| [GetStyles](./getstyles/) | Liest und setzt die Stile für jede Spalte der Tabelle. |
| [SetStyles](./setstyles/) | Liest und setzt die Stile für jede Spalte der Tabelle. |
| [GetIsFormulas](./getisformulas/) | Gibt an, ob die Daten Formeln sind. |
| [SetIsFormulas](./setisformulas/) | Gibt an, ob die Daten Formeln sind. |
| [GetTotalRows](./gettotalrows/) | Liest oder setzt die Gesamtzeilenanzahl, die aus der Datenquelle importiert werden soll. -1 bedeutet alle Zeilen der angegebenen Datenquelle. |
| [SetTotalRows](./settotalrows/) | Liest oder setzt die Gesamtzeilenanzahl, die aus der Datenquelle importiert werden soll. -1 bedeutet alle Zeilen der angegebenen Datenquelle. |
| [GetTotalColumns](./gettotalcolumns/) | Liest oder setzt die Gesamtspaltenanzahl, die aus der Datenquelle importiert werden soll. -1 bedeutet alle Zeilen der angegebenen Datenquelle. |
| [SetTotalColumns](./settotalcolumns/) | Liest oder setzt die Gesamtspaltenanzahl, die aus der Datenquelle importiert werden soll. -1 bedeutet alle Zeilen der angegebenen Datenquelle. |
| [GetColumnIndexes](./getcolumnindexes/) | Liest oder setzt die Spalten (0‑basiert), die aus der Datenquelle importiert werden sollen. null bedeutet, dass alle Spalten importiert werden sollen. |
| [SetColumnIndexes](./setcolumnindexes/) | Liest oder setzt die Spalten (0‑basiert), die aus der Datenquelle importiert werden sollen. null bedeutet, dass alle Spalten importiert werden sollen. |
| [GetDefaultValues](./getdefaultvalues/) | Der Standardwert für den Wert in der Tabelle ist null. |
| [SetDefaultValues](./setdefaultvalues/) | Der Standardwert für den Wert in der Tabelle ist null. |
| [IsHtmlString](./ishtmlstring/) | Gibt an, ob der Wert HTML‑Tags enthält. |
| [SetIsHtmlString](./setishtmlstring/) | Gibt an, ob der Wert HTML‑Tags enthält. |
| [GetCheckMergedCells](./getcheckmergedcells/) | Gibt an, ob zusammengeführte Zellen geprüft werden. |
| [SetCheckMergedCells](./setcheckmergedcells/) | Gibt an, ob zusammengeführte Zellen geprüft werden. |
