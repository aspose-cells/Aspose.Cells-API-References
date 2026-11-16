---
title: "DeleteBlankOptions-Klasse"
linktitle: "DeleteBlankOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DeleteBlankOptions-Klasse. Kapselt das Objekt, das deleteblankoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Stellt die Einstellung zum Löschen leerer Zellen/Zeilen/Spalten dar.

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewDeleteBlankOptions](./newdeleteblankoptions/) | Standardkonstruktor. |
| [NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetEmptyStringAsBlank](./getemptystringasblank/) | Gibt an, ob eine Zelle als leer betrachtet wird, wenn ihr Wert eine leere Zeichenfolge ist. Standardwert ist true. |
| [SetEmptyStringAsBlank](./setemptystringasblank/) | Gibt an, ob eine Zelle als leer betrachtet wird, wenn ihr Wert eine leere Zeichenfolge ist. Standardwert ist true. |
| [GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Gibt an, ob eine Zelle als leer betrachtet wird, wenn sie eine Formel ist und das berechnete Ergebnis null oder eine leere Zeichenfolge ist. Standardwert ist false. |
| [SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Gibt an, ob eine Zelle als leer betrachtet wird, wenn sie eine Formel ist und das berechnete Ergebnis null oder eine leere Zeichenfolge ist. Standardwert ist false. |
| [GetDrawingsAsBlank](./getdrawingsasblank/) | Gibt an, ob zeichnungsbezogene Objekte wie Bild, Form, Diagramm... als leer betrachtet werden. Standardwert ist true. |
| [SetDrawingsAsBlank](./setdrawingsasblank/) | Gibt an, ob zeichnungsbezogene Objekte wie Bild, Form, Diagramm... als leer betrachtet werden. Standardwert ist true. |
| [GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Gibt an, wie zusammengeführte Zellen beim Löschen leerer Zeilen/Spalten verarbeitet werden. |
| [SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Gibt an, wie zusammengeführte Zellen beim Löschen leerer Zeilen/Spalten verarbeitet werden. |
| [GetStartIndex](./getstartindex/) | Gibt den Startzeilen-/Spaltenindex des Bereichs an, der überprüft und leere Zeilen/Spalten gelöscht werden sollen. |
| [SetStartIndex](./setstartindex/) | Gibt den Startzeilen-/Spaltenindex des Bereichs an, der überprüft und leere Zeilen/Spalten gelöscht werden sollen. |
| [GetEndIndex](./getendindex/) | Gibt den Endzeilen-/Spaltenindex (einschließlich) des zu prüfenden Bereichs an, aus dem leere Zeilen/Spalten gelöscht werden sollen. Standardwert ist -1 und -1 bedeutet den maximalen Bereich aller zu prüfenden Objekte (Zellen, Zeichnungen, ...) . |
| [SetEndIndex](./setendindex/) | Gibt den Endzeilen-/Spaltenindex (einschließlich) des zu prüfenden Bereichs an, aus dem leere Zeilen/Spalten gelöscht werden sollen. Standardwert ist -1 und -1 bedeutet den maximalen Bereich aller zu prüfenden Objekte (Zellen, Zeichnungen, ...) . |
| [GetUpdateReference](./getupdatereference/) | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |
| [SetUpdateReference](./setupdatereference/) | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | Liest/setzt den Monitor zur Verfolgung von Änderungen, die durch die Löschung verursacht werden. |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | Liest/setzt den Monitor zur Verfolgung von Änderungen, die durch die Löschung verursacht werden. |
