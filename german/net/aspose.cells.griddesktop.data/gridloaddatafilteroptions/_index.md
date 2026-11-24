---
title: "Enum GridLoadDataFilterOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.Data.GridLoadDataFilterOptions enum. Stellt die Optionen zum Filtern von Daten beim Laden einer Arbeitsmappe aus einer Vorlage dar"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridloaddatafilteroptions/
---
## GridLoadDataFilterOptions enumeration

Stellt die Optionen zum Filtern von Daten beim Laden einer Arbeitsmappe aus einer Vorlage dar.

```csharp
public enum GridLoadDataFilterOptions
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| All | `2147483647` | Alle laden |
| CellBlank | `1` | Lade Zellen, deren Wert leer ist |
| CellString | `2` | Lade Zellen, deren Wert ein Text ist |
| CellNumeric | `4` | Lade Zellen, deren Wert numerisch ist (einschließlich Datum/Zeit) |
| CellError | `8` | Lade Zellen, deren Wert ein Fehler ist |
| CellBool | `16` | Lade Zellen, deren Wert bool ist |
| CellValue | `31` | Lade nur Zellenwerte (alle Werttypen) |
| Formula | `32` | Lade Zellformeln. |
| CellData | `67108927` | Lade Zellendaten einschließlich Werte, Formeln und Formatierung |
| Chart | `256` | Lade Diagramme |
| Drawing | `402653952` | Zeichenobjekte (einschließlich Chart, Picture, OleObject und aller anderen Zeichenobjekte) |
| MergedArea | `1024` | Lade zusammengeführte Zellen |
| ConditionalFormatting | `2048` | Lade bedingte Formatierung |
| DataValidation | `4096` | Lade Datenüberprüfungen |
| PivotTable | `8192` | Lade Pivot-Tabellen |
| Table | `16384` | Lade Tabellen |
| Hyperlinks | `32768` | Lade Hyperlinks |
| SheetSettings | `65536` | Lade Einstellungen für das Arbeitsblatt |
| SheetData | `403701759` | Lade alle Daten des Arbeitsblatts, wie Zellen-Daten, Einstellungen, Objekte, ...etc. |
| BookSettings | `1048576` | Lade Einstellungen für die Arbeitsmappe |
| Settings | `1114112` | Lade Einstellungen für Arbeitsmappe und Arbeitsblatt |
| XmlMap | `2097152` | Lade XmlMap |
| Structure | `4194304` | Lade Struktur der Arbeitsmappe |
| DocumentProperties | `8388608` | Lade Dokumenteigenschaften |
| DefinedNames | `16777216` | Lade definierte Namensobjekte |
| VBA | `33554432` | Lade VBA-Projekte |
| Style | `67108864` | Lade Stile für die Zellformatierung |
| Picture | `134217728` | Bilder laden |
| OleObject | `268435456` | OleObjects laden |
| Revision | `536870912` | Versionsprotokolle laden |

### Siehe auch

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


