---
title: "AccessCacheOptions Aufzählung"
linktitle: "AccessCacheOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "AccessCacheOptions Aufzählung. Kapselt das Objekt, das accesscacheoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/accesscacheoptions/
---

## AccessCacheOptions Enum

Cache-Optionen für den Datenzugriff. Mehrere Optionen können mit dem "|"-Operator kombiniert werden.

```go

type AccessCacheOptions int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [None](./none/) | Kein Cache für jeglichen Datenzugriff. |
| [All](./all/) | Wenden Sie alle möglichen Optimierungen für alle Arten des Datenzugriffs in der Arbeitsmappe an. Alle Einstellungen und Daten dürfen während des optimierten Zugriffs nicht geändert werden. |
| [PositionAndSize](./positionandsize/) | Wenden Sie mögliche Optimierungen zum Abrufen der Position und Größe von Objekten (wie z. B. Shape) an. Zeilenhöhen- und Spaltenbreiteneinstellungen dürfen während des optimierten Zugriffs nicht geändert werden. |
| [CellsData](./cellsdata/) | Wenden Sie mögliche Optimierungen zum Abrufen von Zellwerten an. Zellendaten (Daten und Einstellungen von Zelle, Zeile) dürfen während des optimierten Zugriffs nicht geändert werden, es dürfen auch keine neuen Cell/Row-Objekte erstellt werden (wie z. B. durch <see cref=\"Cells.this[int, int]\"/>). |
| [CellDisplay](./celldisplay/) | Wenden Sie mögliche Optimierungen zum Abrufen von darstellungsbezogenen Ergebnissen von Zellen an (<see cref=\"Cell.DisplayStringValue\"/>, <see cref=\"Cell.GetStyle()\"/>, <see cref=\"Cell.GetDisplayStyle()\"/>, usw.). Zellendaten und stilbezogene Objekte (Cell/Row/Column-Stile, Spaltenbreite usw.) dürfen während des optimierten Zugriffs nicht geändert werden. |
| [GetFormula](./getformula/) | Wenden Sie mögliche Optimierungen zum Abrufen von Formeln an. Alle Daten und Einstellungen, die den Formelausdruck beeinflussen können (Name des Arbeitsblatts, Name-Text, Tabellenspalte usw.), dürfen während des optimierten Zugriffs nicht geändert werden. |
| [SetFormula](./setformula/) | Wenden Sie mögliche Optimierungen zum Setzen von Formeln an. Alle Daten und Einstellungen, die den Formelausdruck beeinflussen können (Name des Arbeitsblatts, Name-Text, Tabellenspalte usw.), dürfen während des optimierten Zugriffs nicht geändert werden. |
| [CalculateFormula](./calculateformula/) | Wenden Sie mögliche Optimierungen zur Berechnung von Formeln an. Zellendaten dürfen während des optimierten Zugriffs nicht geändert werden, es dürfen ebenfalls keine neuen Objekte (Cell, Row usw.) erstellt werden (wie z. B. durch <see cref=\"Cells.this[int, int]\"/>). |
| [ConditionalFormatting](./conditionalformatting/) | Wenden Sie mögliche Optimierungen zum Abrufen des Formatierungsergebnisses bedingter Formatierungen an. Alle Daten und Einstellungen, die das Ergebnis bedingter Formatierungen beeinflussen können (Einstellungen der bedingten Formatierungen, abhängige Zellwerte usw.), dürfen während des optimierten Zugriffs nicht geändert werden. |
| [Validation](./validation/) | Wenden Sie mögliche Optimierungen zum Abrufen des Validierungsergebnisses an. Alle Daten und Einstellungen, die das Ergebnis der Validierung beeinflussen können (Einstellungen der Validierung, abhängige Zellwerte usw.), dürfen während des optimierten Zugriffs nicht geändert werden. |
