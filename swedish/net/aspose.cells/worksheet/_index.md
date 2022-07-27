---
title: Worksheet
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar ett enda kalkylblad.
type: docs
weight: 6510
url: /sv/net/aspose.cells/worksheet/
---
## Worksheet class

Kapslar in objektet som representerar ett enda kalkylblad.

```csharp
public class Worksheet : IDisposable
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [ActiveCell](../../aspose.cells/worksheet/activecell) { get; set; } | Hämtar eller ställer in den aktiva cellen i kalkylbladet. |
| [AllowEditRanges](../../aspose.cells/worksheet/alloweditranges) { get; } | Hämtar samlingen tillåt redigeringsintervall i kalkylbladet. |
| [AutoFilter](../../aspose.cells/worksheet/autofilter) { get; } | Representerar autofilter för det angivna kalkylbladet. |
| [BackgroundImage](../../aspose.cells/worksheet/backgroundimage) { get; set; } | Hämtar och ställer in kalkylbladsbakgrundsbild. |
| [Cells](../../aspose.cells/worksheet/cells) { get; } | Får[`Cells`](./cells) samling. |
| [CellWatches](../../aspose.cells/worksheet/cellwatches) { get; } | Hämtar samling av celler på detta kalkylblad som övervakas i "bevakningsfönstret". |
| [Charts](../../aspose.cells/worksheet/charts) { get; } | Får en[`Chart`](../../aspose.cells.charts/chart) samling |
| [CheckBoxes](../../aspose.cells/worksheet/checkboxes) { get; } | Får en[`CheckBox`](../../aspose.cells.drawing/checkbox) samling. |
| [CodeName](../../aspose.cells/worksheet/codename) { get; set; } | Hämtar kalkylbladskodnamn. |
| [Comments](../../aspose.cells/worksheet/comments) { get; } | Får[`Comment`](../comment) samling. |
| [ConditionalFormattings](../../aspose.cells/worksheet/conditionalformattings) { get; } | Hämtar Conditional Formattings i kalkylbladet. |
| [CustomProperties](../../aspose.cells/worksheet/customproperties) { get; } | Hämtar ett objekt som representerar identifieringsinformationen som är associerad med ett kalkylblad. |
| [DisplayRightToLeft](../../aspose.cells/worksheet/displayrighttoleft) { get; set; } | Indikerar om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. Standard är false. |
| [DisplayZeros](../../aspose.cells/worksheet/displayzeros) { get; set; } | Sant om nollvärden visas. |
| [ErrorCheckOptions](../../aspose.cells/worksheet/errorcheckoptions) { get; } | Får felkontrollinställning tillämpad på vissa intervall. |
| [FirstVisibleColumn](../../aspose.cells/worksheet/firstvisiblecolumn) { get; set; } | Representerar första synliga kolumnindex. |
| [FirstVisibleRow](../../aspose.cells/worksheet/firstvisiblerow) { get; set; } | Representerar första synliga radindex. |
| [HasAutofilter](../../aspose.cells/worksheet/hasautofilter) { get; } | Indikerar om detta kalkylblad har autofilter. |
| [HorizontalPageBreaks](../../aspose.cells/worksheet/horizontalpagebreaks) { get; } | Får[`HorizontalPageBreakCollection`](../horizontalpagebreakcollection) samling. |
| [Hyperlinks](../../aspose.cells/worksheet/hyperlinks) { get; } | Får[`HyperlinkCollection`](../hyperlinkcollection) samling. |
| [Index](../../aspose.cells/worksheet/index) { get; } | Hämtar indexet för arket i kalkylbladssamlingen. |
| [IsGridlinesVisible](../../aspose.cells/worksheet/isgridlinesvisible) { get; set; } | Hämtar eller ställer in ett värde som anger om rutnätslinjerna är synliga. Standard är sant. |
| [IsOutlineShown](../../aspose.cells/worksheet/isoutlineshown) { get; set; } | Indikerar om kontur ska visas. |
| [IsPageBreakPreview](../../aspose.cells/worksheet/ispagebreakpreview) { get; set; } | Indikerar om det angivna kalkylbladet visas i normal vy eller förhandsvisning av sidbrytning. |
| [IsProtected](../../aspose.cells/worksheet/isprotected) { get; } | Indikerar om kalkylbladet är skyddat. |
| [IsRowColumnHeadersVisible](../../aspose.cells/worksheet/isrowcolumnheadersvisible) { get; set; } | Hämtar eller ställer in ett värde som anger om kalkylbladet kommer att visa rad- och kolumnrubriker. Standard är sant. |
| [IsRulerVisible](../../aspose.cells/worksheet/isrulervisible) { get; set; } | Indikerar om linjalen är synlig. Den här egenskapen används endast för förhandsvisning av sidbrytning. |
| [IsSelected](../../aspose.cells/worksheet/isselected) { get; set; } | Indikerar om detta kalkylblad är valt när arbetsboken öppnas. |
| [IsVisible](../../aspose.cells/worksheet/isvisible) { get; set; } | Representerar om kalkylbladet är synligt. |
| [ListObjects](../../aspose.cells/worksheet/listobjects) { get; } | Hämtar alla ListObjects i detta kalkylblad. |
| [Name](../../aspose.cells/worksheet/name) { get; set; } | Hämtar eller ställer in namnet på kalkylbladet. |
| [OleObjects](../../aspose.cells/worksheet/oleobjects) { get; } | Representerar en samling av[`OleObject`](../../aspose.cells.drawing/oleobject) i ett kalkylblad. |
| [Outline](../../aspose.cells/worksheet/outline) { get; } | Får dispositionen på detta arbetsblad. |
| [PageSetup](../../aspose.cells/worksheet/pagesetup) { get; } | Representerar sidkonfigurationsbeskrivningen i det här arket. |
| [PaneState](../../aspose.cells/worksheet/panestate) { get; } | Indikerar om rutan har horisontella eller vertikala delningar, och om dessa delningar är frusna. |
| [Pictures](../../aspose.cells/worksheet/pictures) { get; } | Får en[`Picture`](../../aspose.cells.drawing/picture) samling. |
| [PivotTables](../../aspose.cells/worksheet/pivottables) { get; } | Hämtar alla pivottabeller i detta kalkylblad. |
| [Protection](../../aspose.cells/worksheet/protection) { get; } | Representerar de olika typerna av skyddsalternativ som är tillgängliga för ett kalkylblad. Stöder avancerade skyddsalternativ i ExcelXP och högre version. |
| [QueryTables](../../aspose.cells/worksheet/querytables) { get; } | Blir[`QueryTableCollection`](../querytablecollection) i kalkylbladet. |
| [Scenarios](../../aspose.cells/worksheet/scenarios) { get; } | Får samlingen av[`Scenario`](../scenario) . |
| [Shapes](../../aspose.cells/worksheet/shapes) { get; } | Returnerar alla ritningsformer i detta kalkylblad. |
| [ShowFormulas](../../aspose.cells/worksheet/showformulas) { get; set; } | Indikerar om formler eller deras resultat ska visas. |
| [Slicers](../../aspose.cells/worksheet/slicers) { get; } | Hämta Slicer-samlingen i kalkylbladet |
| [SmartTagSetting](../../aspose.cells/worksheet/smarttagsetting) { get; } | Får alla[`SmartTagCollection`](../../aspose.cells.markup/smarttagcollection) objekt i kalkylbladet. |
| [SparklineGroupCollection](../../aspose.cells/worksheet/sparklinegroupcollection) { get; } | Hämtar sparkline-gruppsamlingen i arbetsbladet. |
| [TabColor](../../aspose.cells/worksheet/tabcolor) { get; set; } | Representerar kalkylbladsflikfärg. |
| [TabId](../../aspose.cells/worksheet/tabid) { get; set; } | Anger den interna identifieraren för arket. |
| [TextBoxes](../../aspose.cells/worksheet/textboxes) { get; } | Får en[`TextBox`](../../aspose.cells.drawing/textbox) samling. |
| [Timelines](../../aspose.cells/worksheet/timelines) { get; } | Hämta tidslinjesamlingen i kalkylbladet |
| [TransitionEntry](../../aspose.cells/worksheet/transitionentry) { get; set; } | Indikerar om alternativet Transition Formula Entry (Lotus-kompatibilitet) är aktiverat. |
| [TransitionEvaluation](../../aspose.cells/worksheet/transitionevaluation) { get; set; } | Indikerar om alternativet Transition Formula Evaluation (Lotus-kompatibilitet) är aktiverat. |
| [Type](../../aspose.cells/worksheet/type) { get; set; } | Representerar kalkylbladstyp. |
| [UniqueId](../../aspose.cells/worksheet/uniqueid) { get; set; } | Hämtar och ställer in det unika ID:t, det är samma som {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [Validations](../../aspose.cells/worksheet/validations) { get; } | Hämtar insamlingen av datavalideringsinställning i kalkylbladet. |
| [VerticalPageBreaks](../../aspose.cells/worksheet/verticalpagebreaks) { get; } | Får[`VerticalPageBreakCollection`](../verticalpagebreakcollection) samling. |
| [ViewType](../../aspose.cells/worksheet/viewtype) { get; set; } | Hämtar och ställer in vytypen. |
| [VisibilityType](../../aspose.cells/worksheet/visibilitytype) { get; set; } | Indikerar det synliga tillståndet för detta ark. |
| [Workbook](../../aspose.cells/worksheet/workbook) { get; } | Hämtar arbetsboksobjektet som innehåller detta ark. |
| [Zoom](../../aspose.cells/worksheet/zoom) { get; set; } | Representerar skalningsfaktorn i procent. Det bör vara mellan 10 och 400. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddPageBreaks](../../aspose.cells/worksheet/addpagebreaks)(string) | Lägger till sidbrytning. |
| [AdvancedFilter](../../aspose.cells/worksheet/advancedfilter)(bool, string, string, string, bool) | Filtrerar data med hjälp av komplexa kriterier. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn#autofitcolumn)(int) | Anpassar kolumnbredden automatiskt. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn#autofitcolumn_1)(int, int, int) | Anpassar kolumnbredden automatiskt. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns)() | Autopassar alla kolumner i detta kalkylblad. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_1)(AutoFitterOptions) | Autopassar alla kolumner i detta kalkylblad. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_2)(int, int) | Anpassar kolumnernas bredd automatiskt. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_3)(int, int, AutoFitterOptions) | Anpassar kolumnernas bredd automatiskt. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_4)(int, int, int, int) | Anpassar kolumnernas bredd automatiskt. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_5)(int, int, int, int, AutoFitterOptions) | Anpassar kolumnernas bredd automatiskt. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow)(int) | Anpassar radhöjden automatiskt. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_1)(int, int, int) | Anpassar radhöjden automatiskt. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_2)(int, int, int, AutoFitterOptions) | Anpassar radhöjden automatiskt. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_3)(int, int, int, int) | Autopassar radhöjd i ett rektangelområde. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows)() | Autopassar alla rader i detta kalkylblad. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_1)(AutoFitterOptions) | Autopassar alla rader i detta kalkylblad. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_2)(bool) | Autopassar alla rader i detta kalkylblad. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_3)(int, int) | Autopassar radhöjd i ett intervall. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_4)(int, int, AutoFitterOptions) | Autopassar radhöjd i ett intervall. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula)(string) | Beräknar en formel. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula_2)(CalculationOptions, bool) | Beräknar alla formler i detta kalkylblad. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula_1)(string, CalculationOptions) | Beräknar en formel. |
| [ClearComments](../../aspose.cells/worksheet/clearcomments)() | Rensar alla kommentarer i designerkalkylark. |
| [CloseAccessCache](../../aspose.cells/worksheet/closeaccesscache)(AccessCacheOptions) | Stänger sessionen som använder cachar för att komma åt data i detta kalkylblad. |
| [Copy](../../aspose.cells/worksheet/copy#copy)(Worksheet) | Kopierar innehåll och format från ett annat kalkylblad. |
| [Copy](../../aspose.cells/worksheet/copy#copy_1)(Worksheet, CopyOptions) | Kopierar innehåll och format från ett annat kalkylblad. |
| [Dispose](../../aspose.cells/worksheet/dispose)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes#freezepanes_1)(string, int, int) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes#freezepanes)(int, int, int, int) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [GetFreezedPanes](../../aspose.cells/worksheet/getfreezedpanes)(out int, out int, out int, out int) | Hämtar frysrutorna. |
| [GetPanes](../../aspose.cells/worksheet/getpanes)() | Får fönsterrutorna. |
| [GetPrintingPageBreaks](../../aspose.cells/worksheet/getprintingpagebreaks)(ImageOrPrintOptions) | Får automatiska sidbrytningar. |
| [GetSelectedRanges](../../aspose.cells/worksheet/getselectedranges)() | Hämtar valda cellintervall i designerkalkylarket. |
| [MoveTo](../../aspose.cells/worksheet/moveto)(int) | Flyttar arket till en annan plats i kalkylarket. |
| [Protect](../../aspose.cells/worksheet/protect#protect)(ProtectionType) | Skyddar kalkylblad. |
| [Protect](../../aspose.cells/worksheet/protect#protect_1)(ProtectionType, string, string) | Skyddar kalkylblad. |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables)() | Uppdaterar alla pivottabeller i detta arbetsblad. |
| [RemoveAllDrawingObjects](../../aspose.cells/worksheet/removealldrawingobjects)() | Tar bort alla ritobjekt i detta kalkylblad. |
| [RemoveAutoFilter](../../aspose.cells/worksheet/removeautofilter)() | Tar bort kalkylbladets automatiska filter. |
| [RemoveSplit](../../aspose.cells/worksheet/removesplit)() | Tar bort delat fönster. |
| [Replace](../../aspose.cells/worksheet/replace)(string, string) | Ersätter alla cellers text med en ny sträng. |
| [SelectRange](../../aspose.cells/worksheet/selectrange)(int, int, int, int, bool) | Väljer ett intervall. |
| [SetVisible](../../aspose.cells/worksheet/setvisible)(bool, bool) | Ställer in de synliga alternativen. |
| [Split](../../aspose.cells/worksheet/split)() | Delar fönster. |
| [StartAccessCache](../../aspose.cells/worksheet/startaccesscache)(AccessCacheOptions) | Startar sessionen som använder cachar för att komma åt data i detta kalkylblad. |
| override [ToString](../../aspose.cells/worksheet/tostring)() | Returnerar en sträng som representerar det aktuella kalkylbladsobjektet. |
| [UnFreezePanes](../../aspose.cells/worksheet/unfreezepanes)() | Frigör rutor i kalkylbladet. |
| [Unprotect](../../aspose.cells/worksheet/unprotect#unprotect)() | Tar bort skyddet av kalkylbladet. |
| [Unprotect](../../aspose.cells/worksheet/unprotect#unprotect_1)(string) | Tar bort skyddet av kalkylbladet. |
| [XmlMapQuery](../../aspose.cells/worksheet/xmlmapquery)(string, XmlMap) | Fråga cellområden som mappade/länkade till den specifika sökvägen för xml-kartan. |

### Exempel

```csharp
[C#]

Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Frys rutor vid "AS40" med 10 rader och 10 kolumner
sheet.FreezePanes("AS40", 10, 10);

//Lägg till en hyperlänk i cell A1
sheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

[Visual Basic]

Dim workbook as Workbook = new Workbook()

Dim sheet as Worksheet = workbook.Worksheets(0)

'Freeze panes at "AS40" with 10 rows and 10 columns
sheet.FreezePanes("AS40", 10, 10)

'Lägg till en hyperlänk i cell A1
sheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com")
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
