---
title: "CellsHelper Klasse"
linktitle: "CellsHelper"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "CellsHelper Klasse. Kapselt das Objekt, das cellshelper in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/cellshelper/
---

## CellsHelper class

Stellt Hilfsfunktionen bereit.

```go

type CellsHelper struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [CellsHelper_GetSignificantDigitsType](./cellshelper_getsignificantdigitstype/) | Liest und schreibt den Standardtyp signifikanter Stellen für die Ausgabe numerischer Werte. Der Standardwert ist SignificantDigitsType.G17. |
| [CellsHelper_SetSignificantDigitsType](./cellshelper_setsignificantdigitstype/) | Liest und schreibt den Standardtyp signifikanter Stellen für die Ausgabe numerischer Werte. Der Standardwert ist SignificantDigitsType.G17. |
| [CellsHelper_GetDPI](./cellshelper_getdpi/) | Liest die DPI des Geräts. |
| [CellsHelper_SetDPI](./cellshelper_setdpi/) | Liest die DPI des Geräts. |
| [CellsHelper_GetTextWidth](./cellshelper_gettextwidth/) | Ermittelt die Breite des Textes in Punkten. |
| [CellsHelper_GetVersion](./cellshelper_getversion/) | Ermittelt die Release-Version. |
| [CellsHelper_CellNameToIndex](./cellshelper_cellnametoindex/) | Liest die Zeilen- und Spaltenindizes einer Zelle anhand ihres Namens. |
| [CellsHelper_CellIndexToName](./cellshelper_cellindextoname/) | Liest den Zellenamen anhand seiner Zeilen- und Spaltenindizes. |
| [CellsHelper_ColumnIndexToName](./cellshelper_columnindextoname/) | Liest den Spaltennamen anhand des Spaltenindex. |
| [CellsHelper_ColumnNameToIndex](./cellshelper_columnnametoindex/) | Liest den Spaltenindex anhand des Spaltennamens. |
| [CellsHelper_RowIndexToName](./cellshelper_rowindextoname/) | Liest den Zeilennamen anhand des Zeilenindex. |
| [CellsHelper_RowNameToIndex](./cellshelper_rownametoindex/) | Liest den Zeilenindex anhand des Zeilennamens. |
| [CellsHelper_GetDateTimeFromDouble](./cellshelper_getdatetimefromdouble/) | Konvertiert den Double-Wert in einen DateTime-Wert. |
| [CellsHelper_GetDoubleFromDateTime](./cellshelper_getdoublefromdatetime/) | Konvertiert den DateTime-Wert in einen Double-Wert. |
| [CellsHelper_GetStartupPath](./cellshelper_getstartuppath/) | Liest oder schreibt den Startpfad, auf den sich einige externe Formelbezüge beziehen. |
| [CellsHelper_SetStartupPath](./cellshelper_setstartuppath/) | Liest oder schreibt den Startpfad, auf den sich einige externe Formelbezüge beziehen. |
| [CellsHelper_GetAltStartPath](./cellshelper_getaltstartpath/) | Liest oder schreibt den alternativen Startpfad, auf den sich einige externe Formelbezüge beziehen. |
| [CellsHelper_SetAltStartPath](./cellshelper_setaltstartpath/) | Liest oder schreibt den alternativen Startpfad, auf den sich einige externe Formelbezüge beziehen. |
| [CellsHelper_GetLibraryPath](./cellshelper_getlibrarypath/) | Liest oder schreibt den Bibliothekspfad, auf den sich einige externe Formelbezüge beziehen. |
| [CellsHelper_SetLibraryPath](./cellshelper_setlibrarypath/) | Liest oder schreibt den Bibliothekspfad, auf den sich einige externe Formelbezüge beziehen. |
| [CellsHelper_GetUsedColors](./cellshelper_getusedcolors/) | Liest alle im Arbeitsbuch verwendeten Farben. |
| [CellsHelper_MergeFiles](./cellshelper_mergefiles/) | Führt mehrere große XLS-Dateien zu einer XLS-Datei zusammen. |
| [CellsHelper_GetCacheFolder](./cellshelper_getcachefolder/) | Liest den Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [CellsHelper_SetCacheFolder](./cellshelper_setcachefolder/) | Setzt den Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [CellsHelper_CreateSafeSheetName_String](./cellshelper_createsafesheetname_string/) | Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen Namen. Wenn der angegebene Blattname den Regeln für Excel-Blattnamen entspricht, wird er zurückgegeben. Andernfalls wird die Zeichenkette abgeschnitten, wenn die Länge das Limit überschreitet, und ungültige Zeichen werden durch ein Leerzeichen (' ') ersetzt, dann wird der wiederhergestellte Zeichenkettenwert zurückgegeben. |
| [CellsHelper_CreateSafeSheetName_String_Char](./cellshelper_createsafesheetname_string_char/) | Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen Namen. Wenn der angegebene Blattname den Regeln für Excel-Blattnamen entspricht, wird er zurückgegeben. Andernfalls wird die Zeichenkette abgeschnitten, wenn die Länge das Limit überschreitet, und ungültige Zeichen werden durch das angegebene Zeichen ersetzt, dann wird der wiederhergestellte Zeichenkettenwert zurückgegeben. |
| [CellsHelper_NeedQuoteInFormula](./cellshelper_needquoteinformula/) | Gibt an, ob der Blattname in einfache Anführungszeichen eingeschlossen werden soll. |
| [CellsHelper_IsCloudPlatform](./cellshelper_iscloudplatform/) | Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud-Plattform wie Azure, AWSLambda usw. ausführen. |
| [CellsHelper_SetIsCloudPlatform](./cellshelper_setiscloudplatform/) | Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud-Plattform wie Azure, AWSLambda usw. ausführen. |
