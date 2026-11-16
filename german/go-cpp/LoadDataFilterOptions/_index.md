---
title: "LoadDataFilterOptions Aufzählung"
linktitle: "LoadDataFilterOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "LoadDataFilterOptions Aufzählung. Kapselt das Objekt, das loaddatafilteroptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/loaddatafilteroptions/
---

## LoadDataFilterOptions Enum

Stellt die Optionen zum Filtern von Daten beim Laden einer Arbeitsmappe aus einer Vorlage dar.

```go

type LoadDataFilterOptions int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [All](./all/) | Alle laden |
| [CellBlank](./cellblank/) | Zellen laden, deren Wert leer ist |
| [CellString](./cellstring/) | Zellen laden, deren Wert ein String ist |
| [CellNumeric](./cellnumeric/) | Zellen laden, deren Wert numerisch ist (einschließlich Datum/Zeit) |
| [CellError](./cellerror/) | Zellen laden, deren Wert ein Fehler ist |
| [CellBool](./cellbool/) | Zellen laden, deren Wert ein Boolescher Wert ist |
| [CellValue](./cellvalue/) | Nur Zellenwerte (alle Werttypen) laden |
| [Formula](./formula/) | Zellformeln laden. |
| [CellData](./celldata/) | Zellendaten laden, einschließlich Werte, Formeln und Formatierung |
| [Chart](./chart/) | Diagramme laden |
| [Drawing](./drawing/) | Zeichnungsobjekte (einschließlich Chart, Picture, OleObject und aller anderen Zeichenobjekte) |
| [MergedArea](./mergedarea/) | Zusammengeführte Zellen laden |
| [ConditionalFormatting](./conditionalformatting/) | Bedingte Formatierung laden |
| [DataValidation](./datavalidation/) | Datenvalidierungen laden |
| [PivotTable](./pivottable/) | Pivot-Tabellen laden |
| [Table](./table/) | Tabellen laden |
| [Hyperlinks](./hyperlinks/) | Hyperlinks laden |
| [SheetSettings](./sheetsettings/) | Einstellungen für das Arbeitsblatt laden |
| [SheetData](./sheetdata/) | Alle Daten des Arbeitsblatts laden, wie Zellendaten, Einstellungen, Objekte, ... usw. |
| [BookSettings](./booksettings/) | Lade Einstellungen für die Arbeitsmappe |
| [Settings](./settings/) | Lade Einstellungen für die Arbeitsmappe und das Arbeitsblatt |
| [XmlMap](./xmlmap/) | Lade XmlMap |
| [Structure](./structure/) | Lade Struktur der Arbeitsmappe |
| [Document_Properties](./document_properties/) | Lade Dokumenteigenschaften |
| [DefinedNames](./definednames/) | Lade definierte Namensobjekte |
| [VBA](./vba/) | Lade VBA-Projekte |
| [Style](./style/) | Lade Stile für die Zellenformatierung |
| [Picture](./picture/) | Lade Bilder |
| [OleObject](./oleobject/) | Lade OleObjects |
| [Revision](./revision/) | Lade Revisionsprotokolle |
