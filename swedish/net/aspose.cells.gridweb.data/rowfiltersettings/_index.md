---
title: "Klass RowFilterSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.RowFilterSettings class. Sammanfattande beskrivning för RowFilter"
type: docs
url: /sv/net/aspose.cells.gridweb.data/rowfiltersettings/
---
## RowFilterSettings class

Sammanfattande beskrivning för RowFilter.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | Filterkriteriesträngen. |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | Aktiverar autofilter. HeaderRow kommer att visa rullgardinsknappar så att användaren kan välja kolumnens värde som ska filtreras. |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | Det sista radnumret i filterintervallet. Om detta värde är satt till -1 används det sista radnumret i bladet. |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | Radnumret för rubriken som kommer att visa filterrullgardinsknappar. |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | Startradnumret i filterintervallet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | Bygger kriteriesträng från autofilterinställningar. |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | Rensar alla filterinställningar och visar alla rader. |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | Specificerar ett anpassat filter. |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | Filtrerar rader med hjälp av kriteriesträng. |

### Anmärkningar

OBS: Denna klass är nu föråldrad. Klassen kommer att tas bort efter 6 månader från augusti 2014. du kan använda GridWorksheet AddAutoFilter/FilterString för autofilter-/anpassade filterinställningar. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


