---
title: "Class WorksheetDesign"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.WorksheetDesign klass. Ärvd från WebWorksheet. Används endast under designtid"
type: docs
url: /sv/net/aspose.cells.gridweb/worksheetdesign/
---
## WorksheetDesign class

Arv från WebWorksheet. Endast för designtid.

```csharp
public class WorksheetDesign : WebWorksheet
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WorksheetDesign](worksheetdesign/#constructor)() | Standardkonstruktor. |
| [WorksheetDesign](worksheetdesign/#constructor_1)(MainWeb, GridWorksheet) | konstruktorn med MainWeb och GridWorksheet |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Bind kollektionskolumner.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | Det faktiska bindande datakällobjektet vid körning. Det är ett DataView-objekt när DataSource-egenskapen är ett DataSet, DataTable eller DataView-objekt.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | I databindningsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | I databindningsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } | (Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Hämtar [`WebCells`](../../aspose.cells.gridweb.data/webcells/).(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } | (Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Hämtar antalet bindningsrader i databindningsläge.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Hämtar eller anger DataMember från den flermedlems‑datakällan. Vanligtvis representerar den ett DataTable‑objekt i ett DataSet.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Hämtar eller anger DataSource. Vanligtvis är det ett DataSet‑objekt.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | I databindningsläge indikerar om kolumnrubriktexter ska skapas i bladet.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Hämtar HyperlinkCollection‑samlingen.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Hämtar indexet för sig själv inom kalkylbladen.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Hämtar eller anger om kalkylbladet är skyddat. När ett kalkylblad är skyddat kan inte alla celler redigeras förutom de celler vars IsLocked‑egenskap är falsk.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Hämtar eller anger namnet på bladet.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } | (Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Hämtar samlingen för datavalideringsinställningar i kalkylbladet.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Indikerar om detta bladnamn visas i bladflikarna i kontrollen.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int) | Anpassar automatiskt kolumnbredden.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int, int, int) | Anpassar automatiskt kolumnbredden. Denna metod anpassar en kolumn baserat på innehållet i ett cellintervall inom kolumnen från startRow till endRow. AutoFitColumn är en inexakt funktion.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Avbryter och tar bort den nylagda bindningsraden.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Bekräftar den nylagda bindningsraden och lägger till den i datakällan.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Kopierar från ett annat kalkylbladsobjekt.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Efter att ha ställt in en datakälla för kalkylbladet, anropa denna metod för att automatiskt generera bindningskolumnerna.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Skapar en ny bindningsrad och binder den till datakällan.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Skapar delsumma i bladet.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Bind bladet till datakällan.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Tar bort en bunden rad.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Fryser rutor vid den angivna cellen i arbetsbladet.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int) | Grupperar rader.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int, bool) | Grupperar rader.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Gör alla celler redigerbara.detta är ett utökat attribut(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Gör alla celler skrivskyddade.detta är ett utökat attribut, observera att detta attribut inte kan behållas i den faktiska cellen, om du vill behålla skyddet vänligen använd setProtect(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Gör ett område av celler redigerbara. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör alla celler skrivskyddade genom att anropa metoden SetAllCellsReadonly. Anropa sedan denna metod för att ange intervallet av celler som ska vara redigerbara(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Gör ett område av celler skrivskyddade. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Först gör alla celler redigerbara genom att anropa metoden SetAllCellsEditable. Anropa sedan denna metod för att ange intervallet av celler som ska vara skrivskyddade(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Avfrostar rutor i arbetsbladet.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Avgrupperar rader.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Uppdaterar bindningsdatakällans post egenskapsvärde enligt cellens värde.(Ärvd från [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

### Se även

* class [WebWorksheet](../../aspose.cells.gridweb.data/webworksheet/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


