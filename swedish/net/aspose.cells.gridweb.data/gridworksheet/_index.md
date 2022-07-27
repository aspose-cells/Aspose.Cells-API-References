---
title: GridWorksheet
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar ett enda kalkylblad.
type: docs
weight: 570
url: /sv/net/aspose.cells.gridweb.data/gridworksheet/
---
## GridWorksheet class

Kapslar in objektet som representerar ett enda kalkylblad.

```csharp
public class GridWorksheet : Control, ISerializable
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell) { get; set; } |  |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage) { get; set; } | Hämtar och ställer in kalkylbladsbakgrundsbild. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns) { get; } | Bind kolumnsamling. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource) { get; } | Det faktiskt bindande datakällans objekt vid körning. Det är ett DataView-objekt när DataSource-egenskapen är ett DataSet-, DataTable- eller DataView-objekt. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn) { get; set; } | I databindningsläge anger BindStartRow och BindStartColumn positionen för rutnätet för att binda till datakällan. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow) { get; set; } | I databindningsläge anger BindStartRow och BindStartColumn positionen för rutnätet för att binda till datakällan. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells) { get; } |  |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename) { get; } | Representerar kalkylbladets kodnamn. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows) { get; set; } | Hämtar numret på bindningsraderna i databindningsläge. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember) { get; set; } | Hämtar eller ställer in DataMember från datakällan med flera medlemmar. Vanligtvis representerar den ett DataTable-objekt i en DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource) { get; set; } | Hämtar eller ställer in DataSource. Vanligtvis är det ett DataSet-objekt. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft) { get; set; } |  |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros) { get; set; } | Sant om nollvärden visas. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader) { get; set; } | I databindningsläge, indikerar om rubriker för bindningskolumnrubriker ska skapas i arket. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn) { get; set; } |  |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow) { get; set; } |  |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell) { get; set; } |  |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks) { get; } | FårHyperlinkCollection samling. |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index) { get; } |  |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible) { get; set; } | Hämtar eller ställer in ett värde som anger om rutnätslinjerna är synliga. Standard är sant. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow) { get; set; } | Indikerar om sammanfattningsraden kommer att placeras under detaljraderna i konturen. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name) { get; set; } | Hämtar eller ställer in namnet på kalkylbladet. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown) { get; set; } | Indikerar om kontur visas. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures) { get; } | Får en[`Pictures`](./pictures) samling. |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables) { get; } | Hämtar pivottabellerna i kalkylbladet. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected) { get; set; } | Indikerar om detta kalkylblad är valt när arbetsboken öppnas. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes) { get; } | Får en[`Pictures`](./pictures) samling. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight) { get; set; } | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i poängenhet. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels) { get; set; } | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i pixelenhet. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor) { get; set; } | Representerar kalkylbladsflikfärg. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations) { get; } | Hämtar insamlingen av datavalideringsinställning i kalkylbladet. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible) { get; set; } | Indikerar om detta arks namn visas i kontrollens arkflikar. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook) { get; } |  |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom) { get; set; } |  |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter)(int, int, int) | Anger intervallet som det angivna autofiltret gäller. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter)(int, string) | Lägg till anpassat filter för den angivna raden. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn#autofitcolumn)(int) | Anpassar kolumnbredden automatiskt. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn#autofitcolumn_1)(int, int, int) | Anpassar kolumnbredden automatiskt. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow#autofitrow)(int) | Anpassar radhöjden automatiskt. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow#autofitrow_1)(int, int, int) | Anpassar radhöjden automatiskt. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow#autofitrow_2)(int, int, int, int) | Autopassar radhöjd i ett rektangelområde. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows#autofitrows)() | Autopassar alla rader i detta kalkylblad. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows#autofitrows_1)(bool) | Autopassar alla rader i detta kalkylblad. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows#autofitrows_2)(int, int) | Autopassar radhöjd i ett intervall. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula)(string) | Beräknar en formel. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow)() | Avbryter och tar bort den nya tillagda bindningsraden. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments)() | Rensar alla kommentarer i designerkalkylark. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow)() | Bekräftar den nya tillagda bindningsraden och lägger till den i datakällan. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy)(GridWorksheet) | Kopierar innehåll och format från ett annat kalkylblad. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns)() | Efter att ha ställt in en datakälla för kalkylbladet, anrop den här metoden för att generera bindningskolumnerna automatiskt. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow)() | Skapar en ny bindningsrad och binder till datakällan. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal#createsubtotal)(int, int, int, SubtotalFunction, int[]) | Skapar delsumma i arket. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Skapar delsumma i arket. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind)() | Bind arket till datakällan. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate)(AccessDataSource) | Bind arket till datakällan. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow)(int) | Tar bort en bindningsrad. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring)(int, string) | Ställer in filtret för column.notice vi ska anropa AddAutoFilter innan anrop av filterString Filterkriteriesträngen. Observera att vi använder komma-&gt;"," som split char, så cellvärdet du vill filtrera ska inte innehålla med comma filterString(10,"123,456") betyder att kolumn 10 ska innehålla 123 eller 456, filterString(10,"123" ) betyder att kolumn 10 ska innehålla 123 värdedelad med kommatecken, t.ex. 123 456 789 eller abc |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes#freezepanes_1)(string, int, int) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes#freezepanes)(int, int, int, int) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption)(int) | Hämtar kolumntexten. Om bildtexten inte är inställd returneras tom sträng. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip)(int) | Hämtar kolumnrubrikens verktygstipstext. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly)(int) | Hämtas om en kolumn är skrivskyddad. detta är en utökad metod för GridWeb specifikt, den kommer inte att behålla och träda i kraft i själva excel file |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes)(out int, out int, out int, out int) | Hämtar frysrutorna. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly)(int, int) | Får om cellen är skrivskyddad. Detta är ett utökat attribut för GridWeb, det kommer inte att behållas i faktiska excel file |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption)(int) | Hämtar radtexten. Om bildtexten inte är inställd returneras tom sträng. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip)(int) | Hämtar radhuvudets verktygstipstext. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly)(int) | Hämtas om en rad är skrivskyddad. detta är en utökad metod för GridWeb specifikt, den kommer inte att behålla och påverka i själva excel file |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows)(int, int, bool) | Grupper rader. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected)() | Indikerar om kalkylbladet är skyddat. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto)(int) | Flyttar arket till en annan plats i kalkylarket. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter)() | Uppdatera automatiska filter för att dölja eller visa raderna. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter)() | Ta bort kalkylbladets automatiska filter. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal)() | Tar bort delsumma som skapats med metoden CreateSubtotal i arket. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter)(int) | Heltalsförskjutningen för fältet som du vill använda, baserat på den första filterkolumnen (från vänster i listan; fältet längst till vänster är fältet 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable)() | Gör alla celler redigerbara. Detta är utökat attribut |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly)() | Gör alla celler skrivskyddade. detta utökas attribut Observera att detta attribut inte kan behållas i den faktiska cellen, om du vill behålla skydda använd setProtect |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption)(int, string) | Ställer in rubriken för kolumnen. Observera att detta är ett tilläggsattribut och kan inte behållas i excel file |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip)(int, string) | Ställer in kolumnrubrikens verktygstipstext. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly)(int, bool) | Ställer in en kolumn till skrivskyddad så att användaren inte kan ta bort den från klientsidan. detta är en utökad metod för GridWeb specifikt, den kommer inte att behålla och träda i kraft i själva excel file |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange)(int, int, int, int) | Gör ett cellintervall redigerbart. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör alla celler läsbara genom att anropa SetAllCellsReadonly-metoden. anrop sedan den här metoden för att ange cellintervallet som ska kunna redigeras |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly)(int, int, bool) | Anger om cellen är skrivskyddad. Detta är ett utökat attribut för GridWeb, det kommer inte att finnas kvar i den faktiska excel-filen |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect)() | Skyddar kalkylblad. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange)(int, int, int, int) | Gör ett cellområde skrivskyddat. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör först alla celler redigerbara genom att anropa SetAllCellsEditable-metoden. anropa sedan den här metoden för att ange cellintervallet som ska vara skrivskyddat |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption)(int, string) | Ställer in bildtexten för raden. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip)(int, string) | Ställer in radrubrikens verktygstipstext. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly)(int, bool) | Ställer in en rad till skrivskyddad så att användaren inte kan ta bort den från klientsidan. detta är en utökad metod för GridWeb specifikt, den kommer inte att behålla och träda i kraft i själva excel file |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes)() | Frigör rutor i kalkylbladet. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows)(int, int) | Delar upp rader. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect)() | avskyddar kalkylblad. |

### Se även

* namnutrymme [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* hopsättning [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
