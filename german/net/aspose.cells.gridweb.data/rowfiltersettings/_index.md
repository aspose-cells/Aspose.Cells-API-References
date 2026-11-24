---
title: "Klasse RowFilterSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.RowFilterSettings Klasse. Zusammenfassende Beschreibung für RowFilter."
type: docs
url: /de/net/aspose.cells.gridweb.data/rowfiltersettings/
---
## RowFilterSettings class

Kurzbeschreibung für RowFilter.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | Die Filterkriterienzeichenkette. |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | Aktiviert die automatische Filterung. Die HeaderRow zeigt Dropdown‑Schaltflächen an, damit der Benutzer den zu filternden Spaltenwert auswählen kann. |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | Die Endzeilennummer des Filterbereichs. Wenn dieser Wert auf -1 gesetzt ist, wird die letzte Zeilennummer des Blatts verwendet. |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | Die Headerzeilennummer, die Dropdown‑Schaltflächen für den Filter anzeigt. |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | Die Startzeilennummer des Filterbereichs. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | Erstellt die Kriterienzeichenkette aus den automatischen Filtereinstellungen. |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | Löscht alle Filtereinstellungen und zeigt alle Zeilen an. |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | Gibt einen benutzerdefinierten Filter an. |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | Filtert Zeilen anhand einer Kriterienzeichenkette. |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Diese Klasse wird nach 6 Monaten seit August 2014 entfernt werden. Sie können GridWorksheet AddAutoFilter/FilterString für Auto‑Filter‑/ benutzerdefinierte Filtereinstellungen verwenden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


