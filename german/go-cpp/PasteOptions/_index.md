---
title: "PasteOptions Klasse"
linktitle: "PasteOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PasteOptions Klasse. Kapselt das Objekt, das PasteOptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pasteoptions/
---

## PasteOptions class

Stellt die Optionen für Spezial‑Einfügen dar.

```go

type PasteOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewPasteOptions](./newpasteoptions/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetPasteType](./getpastetype/) | Der spezielle Einfügetyp. |
| [SetPasteType](./setpastetype/) | Der spezielle Einfügetyp. |
| [GetShiftFormulasOfShapes](./getshiftformulasofshapes/) | Gibt an, ob Formeln der Formen beim Kopieren von Bereichen verschoben werden sollen. |
| [SetShiftFormulasOfShapes](./setshiftformulasofshapes/) | Gibt an, ob Formeln der Formen beim Kopieren von Bereichen verschoben werden sollen. |
| [GetSkipBlanks](./getskipblanks/) | Gibt an, ob leere Zellen übersprungen werden. |
| [SetSkipBlanks](./setskipblanks/) | Gibt an, ob leere Zellen übersprungen werden. |
| [GetKeepOldTables](./getkeepoldtables/) | Behält die Tabellen im Zielbereich. |
| [SetKeepOldTables](./setkeepoldtables/) | Behält die Tabellen im Zielbereich. |
| [GetOnlyVisibleCells](./getonlyvisiblecells/) | True bedeutet, nur sichtbare Zellen zu kopieren. |
| [SetOnlyVisibleCells](./setonlyvisiblecells/) | True bedeutet, nur sichtbare Zellen zu kopieren. |
| [GetTranspose](./gettranspose/) | True, um Zeilen und Spalten beim Einfügen des Bereichs zu transponieren. Der Standardwert ist False. |
| [SetTranspose](./settranspose/) | True, um Zeilen und Spalten beim Einfügen des Bereichs zu transponieren. Der Standardwert ist False. |
| [GetOperationType](./getoperationtype/) | Liest und setzt den Operationstyp beim Einfügen des Bereichs. |
| [SetOperationType](./setoperationtype/) | Liest und setzt den Operationstyp beim Einfügen des Bereichs. |
| [GetIgnoreLinksToOriginalFile](./getignorelinkstooriginalfile/) | Ignoriere Links zur Originaldatei. |
| [SetIgnoreLinksToOriginalFile](./setignorelinkstooriginalfile/) | Ignoriere Links zur Originaldatei. |
