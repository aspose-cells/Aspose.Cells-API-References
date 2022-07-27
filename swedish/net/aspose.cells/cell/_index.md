---
title: Cell
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar en enskild arbetsbokscell.
type: docs
weight: 230
url: /sv/net/aspose.cells/cell/
---
## Cell class

Kapslar in objektet som representerar en enskild arbetsbokscell.

```csharp
public class Cell
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | Hämtar det booleska värdet som finns i cellen. |
| [Column](../../aspose.cells/cell/column) { get; } | Hämtar kolumnnummer (nollbaserat) för cellen. |
| [Comment](../../aspose.cells/cell/comment) { get; } | Hämtar kommentaren från den här cellen. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | Indikerar om denna cell innehåller en extern länk. Gäller endast när cellen är en formelcell. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | Hämtar DateTime-värdet som finns i cellen. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | Hämtar det formaterade strängvärdet för denna cell efter cellens visningsstil. |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | Får det dubbla värdet som finns i cellen. |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | Hämtar flytvärdet som finns i cellen. |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | Hämtar eller ställer in en formel för[`Cell`](../cell) . |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | Få den språkformaterade formeln för cellen. |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | Hämtar och ställer in html-strängen som innehåller data och vissa format i den här cellen. |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | Hämtar heltalsvärdet som finns i cellen. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | Indikerar om cellformeln är en matrisformel. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | Indikerar cellens formel är och matrisformel och det är den första cellen i matrisen. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | Kontrollerar om värdet på den här cellen är ett fel. |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | Representerar om den angivna cellen innehåller formel. |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | Kontrollerar om en cell är en del av ett sammanslaget område eller inte. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | Indikerar om det inre värdet i denna cell är numeriskt (int, double och datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | Indikerar om cellformeln är en del av delad formel. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | Indikerar om cellens stil är inställd. Om returnera false betyder det att den här cellen har ett standardcellformat. |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | Indikerar om denna cell är en del av tabellformeln. |
| [Name](../../aspose.cells/cell/name) { get; } | Hämtar namnet på cellen. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | Representerar kategoritypen för denna cells nummerformatering. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | Hämtar eller ställer in en R1C1-formel för[`Cell`](../cell) . |
| [Row](../../aspose.cells/cell/row) { get; } | Hämtar radnummer (nollbaserat) för cellen. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | Hämtar cellens delade stilindex i stilpoolen. |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | Hämtar strängvärdet som finns i cellen. Om typen av denna cell är sträng, returnera sedan själva strängvärdet. För andra celltyper kommer det formaterade strängvärdet (formaterat med den angivna stilen för denna cell) att returneras. Det formaterade cellvärdet är detsamma som du kan komma från excel när du kopierar en cell som text (som kopierar cell till textredigerare eller exporterar till csv). |
| [Type](../../aspose.cells/cell/type) { get; } | Representerar cellvärdestyp. |
| [Value](../../aspose.cells/cell/value) { get; set; } | Hämtar värdet som finns i den här cellen. |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | Hämtar det överordnade arbetsbladet. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate#calculate)(CalculationOptions) | Beräknar cellens formel. |
| [Characters](../../aspose.cells/cell/characters)(int, int) | Returnerar ett teckenobjekt som representerar ett teckenintervall i celltexten. |
| [Copy](../../aspose.cells/cell/copy)(Cell) | Kopierar data från en källcell. |
| [Equals](../../aspose.cells/cell/equals#equals)(Cell) | Kontrollerar om detta objekt refererar till samma cell med ett annat cellobjekt. |
| override [Equals](../../aspose.cells/cell/equals#equals_1)(object) | Kontrollerar om detta objekt refererar till samma cell med en annan. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | Hämtar matrisområdet om cellens formel är en matrisformel. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters)() | Returnerar alla teckenobjekt som representerar ett teckenintervall i celltexten. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters_1)(bool) | Returnerar alla teckenobjekt som representerar ett teckenintervall i celltexten. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | Få resultatet av den villkorliga formateringen. |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | Få alla celler vars formel refererar till den här cellen direkt. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation)(bool) | Hämtar alla celler vars beräknade resultat beror på denna cell. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle)() | Hämtar visningsstilen för cellen. Om denna cell också påverkas av andra inställningar såsom villkorlig formatering, listobjekt, etc., kan visningsstilen skilja sig från cell.GetStyle(). |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle_1)(bool) | Hämtar visningsstilen för cellen. Om cellen är villkorligt formaterad är visningsstilen inte samma som cellen.GetStyle(). |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | Hämtar formatvillkor som gäller för den här cellen. |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | Få formeln för den här cellen. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | Fungerar som en hashfunktion för en viss typ. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | Hämtar höjden på värdet i enhet pixlar. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | Hämtar html-strängen som innehåller data och vissa format i den här cellen. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | Returnerar en[`Range`](../range) objekt som representerar ett sammanslaget område. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | Får alla referenser som visas i den här cellens formel. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation)() | Hämtar alla prejudikat (referens till celler i aktuell arbetsbok) som används av denna cells formel när den beräknas. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | Hämtar strängvärdet efter specifik formaterad strategi. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle)() | Hämtar cellstilen. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle_1)(bool) | Om checkBorders är sant, kontrollera om andra cellers gränser kommer att påverka stilen för denna cell. |
| [GetTable](../../aspose.cells/cell/gettable)() | Hämtar tabellen som innehåller denna cell. |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | Får valideringen tillämpad på den här cellen. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | Får valideringsvärdet som tillämpades på den här cellen. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | Hämtar bredden på värdet i enhet pixlar. |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | Indikerar om cellsträngens värde är en rik text. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue)(bool) | Lägger ett booleskt värde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_3)(DateTime) | Lägger in ett DateTime-värde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_1)(double) | Lägger ett dubbelt värde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_2)(int) | Lägger ett heltalsvärde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_4)(object) | Lägger ett objektvärde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_5)(string) | Lägger in ett strängvärde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_6)(string, bool) | Lägger in ett strängvärde i cellen och konverterar värdet till annan datatyp om så är lämpligt. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_7)(string, bool, bool) | Lägger in ett värde i cellen, om så är lämpligt kommer värdet att konverteras till annan datatyp och cellens talformat återställs. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | Ta bort matrisformel. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula)(string, int, int) | Ställer in en matrisformel (äldre matrisformel som anges via CTRL+SHIFT+ENTER i ms excel) till ett cellintervall. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_1)(string, int, int, FormulaParseOptions) | Ställer in en matrisformel till ett cellintervall. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Ställer in en matrisformel till ett cellintervall. |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | Anger RTF-format för cellen. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Ställer in dynamisk matrisformel och får formeln att spilla in i närliggande celler om möjligt. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Ställer in dynamisk matrisformel och får formeln att spilla in i närliggande celler om möjligt. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula_2)(string, object) | Ställ in formeln och värdet för formeln. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula)(string, FormulaParseOptions, object) | Ställ in formeln och värdet för formeln. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula)(string, int, int) | Anger en formel till ett cellintervall. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_1)(string, int, int, FormulaParseOptions) | Anger en formel till ett cellintervall. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Anger en formel till ett cellintervall. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle)(Style) | Ställer in cellstilen. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_2)(Style, bool) | Använd cellformatet. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_1)(Style, StyleFlag) | Använd cellformatet. |
| override [ToString](../../aspose.cells/cell/tostring)() | Returnerar en sträng som representerar det aktuella cellobjektet. |

### Exempel

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Sätt in en sträng i en cell
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
//Sätt ett heltal i en cell
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

//Sätt en dubbel i en cell
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

//Sätt in en formel i en cell
cell = cells["D1"];
cell.Formula = "=B1 + C1";

//Sätt en kombinerad formel: "summa(medelvärde(b1,c1), b1)" till cellen vid b2
cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

//Ange stil för en cell
Style style = cell.GetStyle();
//Ställ in bakgrundsfärg
style.BackgroundColor = Color.Yellow;
//Ange format för en cell
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

'Sätt en sträng i en cell
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
//Sätt ett heltal i en cell
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

//Sätt en dubbel i en cell
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

//Sätt in en formel i en cell
cell = cells("D1")
cell.Formula = "=B1 + C1"

//Sätt en kombinerad formel: "summa(medelvärde(b1,c1), b1)" till cellen vid b2
cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
//Ange stil för en cell
Dim style as Style = cell.GetStyle()

//Ställ in bakgrundsfärg
style.BackgroundColor = Color.Yellow
//Ange teckensnitt för en cell
style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
