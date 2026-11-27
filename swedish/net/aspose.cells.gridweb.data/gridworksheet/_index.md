---
title: "Klass GridWorksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.GridWorksheet-klass. Inkapslar objektet som representerar ett enskilt kalkylblad"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridworksheet/
---
## GridWorksheet class

Inkapslar objektet som representerar ett enskilt arbetsblad.

```csharp
public class GridWorksheet : Control, ISerializable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell/) { get; set; } | Hämtar eller anger den aktiva cellen i kalkylbladet. |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage/) { get; set; } | Hämtar och anger kalkylbladets bakgrundsbild. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns/) { get; } | Bind kolumnsamling. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource/) { get; } | Det faktiska bindningsdatakällobjektet vid körning. Det är ett DataView-objekt när DataSource-egenskapen är ett DataSet-, DataTable- eller DataView-objekt. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn/) { get; set; } | I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow/) { get; set; } | I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells/) { get; } | Hämtar [`GridCell`](../gridcell/) samlingen. |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename/) { get; } | Representerar kalkylbladets kodnamn. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments/) { get; } | Hämtar [`GridComment`](../gridcomment/) samlingen. |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows/) { get; set; } | Hämtar antalet bindningsrader i datakopplingsläge. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember/) { get; set; } | Hämtar eller anger DataMember från den flermedlems‑DataSource. Generellt representerar den ett DataTable‑objekt från ett DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource/) { get; set; } | Hämtar eller anger DataSource. Vanligtvis är det ett DataSet-objekt. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft/) { get; set; } | Anger om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. Standard är falskt. |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros/) { get; set; } | Sant om nollvärden visas. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader/) { get; set; } | I data-binding-läge anger den om bindningskolumnrubriker ska skapas i bladet. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn/) { get; set; } | Representerar första synliga kolumnens index. |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow/) { get; set; } | Representerar första synliga radens index. |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell/) { get; set; } | Hämtar eller anger den aktiva cellen i kalkylbladet. |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks/) { get; } | Hämtar [`GridHyperlinkCollection`](../gridhyperlinkcollection/) samlingen. |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index/) { get; } | Hämtar indexet för bladet i kalkylblads samlingen. |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible/) { get; set; } | Hämtar eller anger ett värde som indikerar om rutnätslinjerna är synliga. Standard är true. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow/) { get; set; } | Anger om sammanfattningsraden kommer att placeras under detaljraderna i konturen. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name/) { get; set; } | Hämtar eller anger namnet på arbetsbladet. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown/) { get; set; } | Anger om outline ska visas. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures/) { get; } | Hämtar en [`Pictures`](./pictures/) samling. |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables/) { get; } | Hämtar pivotTables i arbetsbladet. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected/) { get; set; } | Anger om detta kalkylblad är valt när arbetsboken öppnas. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes/) { get; } | Hämtar en [`Pictures`](./pictures/) samling. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight/) { get; set; } | Hämtar eller anger standardradhöjden i detta kalkylblad, i enheten punkter. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels/) { get; set; } | Hämtar eller anger standardradhöjden i detta kalkylblad, i enheten pixlar. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor/) { get; set; } | Representerar färgen på arbetsbladsfliken. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations/) { get; } | Hämtar datavalideringsinställningssamlingen i arbetsbladet. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible/) { get; set; } | Anger om detta bladnamn visas i bladflikarna i kontrollen. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook/) { get; } | Hämtar [`GridWorkbook`](../gridworkbook/) objektet i arbetsbladsamlingen. |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom/) { get; set; } | Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter/)(int, int, int) | Ställer in intervallet som den angivna AutoFiltern gäller för. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter/)(int, string) | Lägg till anpassat filter för den angivna raden. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn)(int) | Anpassar automatiskt kolumnbredden. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Anpassar automatiskt kolumnbredden. |
| [AutoFitColumns](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumns/)() |  |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow)(int) | Anpassar automatiskt radhöjden. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_1)(int, int, int) | Anpassar automatiskt radhöjden. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_2)(int, int, int, int) | Anpassar automatiskt radhöjden i ett rektangulärt område. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows)() | Anpassar automatiskt alla rader i detta kalkylblad. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_1)(bool) | Anpassar automatiskt alla rader i detta kalkylblad. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_2)(int, int) | Anpassar automatiskt radhöjden i ett område. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula/)(string) | Beräknar en formel. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow/)() | Avbryter och tar bort den nyligen tillagda bindningsraden. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments/)() | Rensar alla kommentarer i designerns kalkylblad. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow/)() | Bekräftar den nyligen tillagda bindningsraden och lägger till den i datakällan. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy/)(GridWorksheet) | Kopierar innehåll och format från ett annat kalkylblad. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns/)() | Efter att ha ställt in en datasource för arbetsbladet, anropa den här metoden för att automatiskt generera bindningskolumnerna. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow/)() | Skapar en ny bindningsrad och binder den till datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal)(int, int, int, SubtotalFunction, int[]) | Skapar delsumma i bladet. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Skapar delsumma i bladet. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind/)() | Bind bladet till DataSource. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate/)(AccessDataSource) | Bind bladet till DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow/)(int) | Tar bort en bindningsrad. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring/)(int, string) | Ställer in filtret för kolumnen. Observera att vi ska anropa AddAutoFilter innan filterString anropas. Filterkriteriesträngen. Observera att vi använder komma-&gt;"," som avgränsare, så cellvärdet du vill filtrera får inte innehålla komma. filterString(10,"123,456") betyder att kolumn 10 ska innehålla 123 eller 456, filterString(10,"123") betyder att kolumn 10 ska innehålla 123. Kolumnindexvärdet separeras med komma, t.ex. 123,456,789 eller abc. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes_1)(string, int, int) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes)(int, int, int, int) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption/)(int) | Hämtar kolumnrubriken. Om rubriken inte är angiven returneras en tom sträng. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip/)(int) | Hämtar verktygstipstexten för columnheader. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly/)(int) | Hämtar om en kolumn är skrivskyddad. Detta är en utökad metod i GridWeb specifikt, den kommer inte att sparas eller påverka den faktiska Excel-filen. |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes/)(out int, out int, out int, out int) | Hämtar frysfönstren. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly/)(int, int) | Hämtar om cellen är skrivskyddad. Detta är ett utökat attribut i GridWeb, det kommer inte att sparas i den faktiska Excel-filen. |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption/)(int) | Hämtar radrubriken. Om rubriken inte är angiven returneras en tom sträng. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip/)(int) | Hämtar verktygstipstexten för rowheader. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly/)(int) | Hämtar om en rad är skrivskyddad. Detta är en utökad metod i GridWeb specifikt, den kommer inte att sparas eller påverka den faktiska Excel-filen. |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows/)(int, int, bool) | Grupperar rader. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected/)() | Anger om kalkylbladet är skyddat. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto/)(int) | Flyttar bladet till en annan plats i kalkylbladet. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter/)() | Uppdatera autofilter för att dölja eller visa raderna. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter/)() | Ta bort autofiltret i kalkylbladet. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal/)() | Tar bort delsumma som skapats av metoden CreateSubtotal i bladet. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter/)(int) | Det heltalsavståndet för fältet som du vill tillämpa, baserat på den första filterkolumnen (från vänster i listan; det vänstra fältet är fält 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable/)() | Gör alla celler redigerbara. Detta är ett utökat attribut |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly/)() | Gör alla celler skrivskyddade. Detta är ett utökat attribut, observera att detta attribut inte kan behållas i den faktiska cellen; om du vill behålla skyddet, använd setProtect. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption/)(int, string) | Ställer in rubriken för kolumnen. Observera att detta är ett extensionsattribut och inte kan sparas i Excel-filen. |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip/)(int, string) | Ställer in verktygstipptexten för kolumnrubriken. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly/)(int, bool) | Ställer in en kolumn som skrivskyddad så att användaren inte kan ta bort den från klientsidan. Detta är en utökad metod för GridWeb specifikt, den kommer inte att sparas eller ha effekt i den faktiska Excel-filen. |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange/)(int, int, int, int) | Gör ett område av celler redigerbara. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör alla celler skrivskyddade genom att anropa metoden SetAllCellsReadonly. Anropa sedan denna metod för att specificera vilka cellområden som ska vara redigerbara. |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly/)(int, int, bool) | Ställer in om cellen är skrivskyddad. Detta är ett utökat attribut för GridWeb, det kommer inte att sparas i den faktiska Excel-filen. |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect/)() | Skyddar kalkylbladet. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange/)(int, int, int, int) | Gör ett område av celler skrivskyddade. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Först gör alla celler redigerbara genom att anropa metoden SetAllCellsEditable. Anropa sedan denna metod för att specificera vilka cellområden som ska vara skrivskyddade. |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption/)(int, string) | Ställer in rubriken för raden. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip/)(int, string) | Ställer in verktygstipptexten för radrubriken. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly/)(int, bool) | Ställer in en rad som skrivskyddad så att användaren inte kan ta bort den från klientsidan. Detta är en utökad metod för GridWeb specifikt, den kommer inte att sparas eller ha effekt i den faktiska Excel-filen. |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes/)() | Låser upp fönstren i kalkylbladet. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows/)(int, int) | Avgrupperar rader. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect/)() | Tar bort skyddet från kalkylbladet. |

## Händelser

| Namn | Beskrivning |
| --- | --- |
| event [InitializeNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/initializenewbindrow/) | Uppstår när kalkylbladet har skapat en ny bindrad och den behöver initieras. |

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


