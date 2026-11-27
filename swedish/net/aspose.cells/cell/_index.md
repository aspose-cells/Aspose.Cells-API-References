---
title: "Klass Cell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Cell klass. Inkapslar objektet som representerar en enskild arbetsbokscell"
type: docs
url: /sv/net/aspose.cells/cell/
---
## Cell class

Inkapslar objektet som representerar en enskild Workbook-cell.

```csharp
public class Cell
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue/) { get; } | Hämtar det booleska värdet som finns i cellen. |
| [Column](../../aspose.cells/cell/column/) { get; } | Hämtar kolumnnumret (nollbaserat) för cellen. |
| [Comment](../../aspose.cells/cell/comment/) { get; } | Hämtar kommentaren för den här cellen. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink/) { get; } | Anger om den här cellen innehåller en extern länk. Gäller endast när cellen är en formelcell. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue/) { get; } | Hämtar DateTime‑värdet som finns i cellen. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue/) { get; } | Hämtar det formaterade strängvärdet för den här cellen enligt cellens visningsstil. |
| [DoubleValue](../../aspose.cells/cell/doublevalue/) { get; } | Hämtar dubbelvärdet som finns i cellen. |
| [EmbeddedImage](../../aspose.cells/cell/embeddedimage/) { get; set; } | Hämtar och anger den inbäddade bilden i cellen. |
| [FloatValue](../../aspose.cells/cell/floatvalue/) { get; } | Hämtar flyttalsvärdet som finns i cellen. |
| [Formula](../../aspose.cells/cell/formula/) { get; set; } | Hämtar eller anger en formel för `Cell`. |
| [FormulaLocal](../../aspose.cells/cell/formulalocal/) { get; set; } | Hämta den lokalanpassade formeln för cellen. |
| [HasCustomFunction](../../aspose.cells/cell/hascustomfunction/) { get; } | Kontrollerar om det finns en anpassad funktion (ej stödd funktion) i cellens formel. |
| [HasCustomStyle](../../aspose.cells/cell/hascustomstyle/) { get; } | Anger om den här cellen har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från motsvarande rad, kolumn eller arbetsbok). |
| [HtmlString](../../aspose.cells/cell/htmlstring/) { get; set; } | Hämtar och anger html-strängen som innehåller data och vissa format i den här cellen. |
| [IntValue](../../aspose.cells/cell/intvalue/) { get; } | Hämtar heltalsvärdet som finns i cellen. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula/) { get; } | Anger om cellens formel är en matrisformel. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader/) { get; } | Anger att cellens formel är en matrisformel och att den är den första cellen i matrisen. |
| [IsCheckBoxStyle](../../aspose.cells/cell/ischeckboxstyle/) { get; set; } | Anger om cellen är inställd som en kryssruta. |
| [IsDynamicArrayFormula](../../aspose.cells/cell/isdynamicarrayformula/) { get; } | Anger om cellens formel är en dynamisk matrisformel (true) eller en äldre matrisformel (false). |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue/) { get; } | Kontrollerar om värdet i den här cellen är ett fel. |
| [IsFormula](../../aspose.cells/cell/isformula/) { get; } | Anger om den angivna cellen innehåller en formel. |
| [IsInArray](../../aspose.cells/cell/isinarray/) { get; } | (**Obsolete.**) Anger om cellens formel är en matrisformel. |
| [IsInTable](../../aspose.cells/cell/isintable/) { get; } | (**Obsolete.**) Anger om den här cellen är en del av en tabellformel. |
| [IsMerged](../../aspose.cells/cell/ismerged/) { get; } | Kontrollerar om en cell är en del av ett sammanslaget område eller inte. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue/) { get; } | Anger om värdet i den här cellen är numeriskt (int, double och datetime). |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula/) { get; } | Anger om cellens formel är en del av en delad formel. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset/) { get; } | Anger om cellens stil är angiven. Om den returnerar false betyder det att cellen har ett standardformat. |
| [IsTableFormula](../../aspose.cells/cell/istableformula/) { get; } | Anger om den här cellen är en del av en tabellformel. |
| [Name](../../aspose.cells/cell/name/) { get; } | Hämtar cellens namn. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype/) { get; } | Anger kategoritypen för den här cellens talformat. |
| [Picture](../../aspose.cells/cell/picture/) { get; } | Hämtar en [`Picture`](../../aspose.cells.drawing/picture/) instans för att representera den inbäddade bilden i den här cellen eller null om det inte finns någon inbäddad bild för den här cellen. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula/) { get; set; } | Hämtar eller anger en R1C1-formel för `Cell`. |
| [Row](../../aspose.cells/cell/row/) { get; } | Hämtar radnumret (nollbaserat) för cellen. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex/) { get; } | Hämtar cellens delade stilindex i stilpoolen. |
| [StringValue](../../aspose.cells/cell/stringvalue/) { get; } | Hämtar strängvärdet som finns i cellen. Om cellens typ är sträng returneras själva strängvärdet. För andra celltyper returneras det formaterade strängvärdet (formaterat med den angivna stilen för den här cellen). Det formaterade cellvärdet är detsamma som vad du kan få i Excel när du kopierar en cell som text (t.ex. kopierar cellen till en textredigerare eller exporterar till CSV). |
| [StringValueWithoutFormat](../../aspose.cells/cell/stringvaluewithoutformat/) { get; } | (**Obsolete.**) Hämtar cellens värde som sträng utan någon formatering. |
| [Type](../../aspose.cells/cell/type/) { get; } | Anger cellvärdestyp. |
| [Value](../../aspose.cells/cell/value/) { get; set; } | Hämtar/anger värdet som finns i den här cellen. |
| [Worksheet](../../aspose.cells/cell/worksheet/) { get; } | Hämtar det överordnade kalkylbladet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate/)(CalculationOptions) | Beräknar cellens formel. |
| [Characters](../../aspose.cells/cell/characters/)(int, int) | Returnerar ett Characters-objekt som representerar ett teckenintervall inom cellens text. |
| [Copy](../../aspose.cells/cell/copy/)(Cell) | Kopierar data från en källcell. |
| [Equals](../../aspose.cells/cell/equals/#equals)(Cell) | Kontrollerar om detta objekt refererar till samma cell som ett annat cellobjekt. |
| override [Equals](../../aspose.cells/cell/equals/#equals_1)(object) | Kontrollerar om detta objekt refererar till samma cell som ett annat. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange/)() | Hämtar array-intervallet om cellens formel är en arrayformel. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters)() | Returnerar alla Characters-objekt som representerar ett teckenintervall inom cellens text. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters_1)(bool) | Returnerar alla Characters-objekt som representerar ett teckenintervall inom cellens text. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult/)() | Hämta resultatet av den villkorsstyrda formateringen. |
| [GetDependents](../../aspose.cells/cell/getdependents/)(bool) | Hämta alla celler vars formel refererar direkt till denna cell. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation/)(bool) | Hämtar alla celler vars beräknade resultat beror på denna cell. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle)() | Hämtar cellens visningsstil. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_2)(bool) | Hämtar cellens visningsstil. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_1)(BorderType) | Hämtar cellens visningsstil. |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions/)() | Hämtar formatvillkor som gäller för denna cell. |
| [GetFormula](../../aspose.cells/cell/getformula/)(bool, bool) | Hämta formeln för denna cell. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode/)() | Fungerar som en hash-funktion för en viss typ. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue/)() | Hämtar värdets höjd i pixelenheter. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring/)(bool) | Hämtar HTML-strängen som innehåller data och vissa format i denna cell. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs)() | (**Obsolete.**) Hämta alla celler som refererar till denna cell direkt och som måste uppdateras när denna cell ändras. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs_1)(bool) | (**Obsolete.**) Hämta alla celler som kommer att uppdateras när denna cell ändras. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange/)() | Returnerar ett [`Range`](../range/) objekt som representerar ett sammanslaget område. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents/)() | Hämtar alla referenser som förekommer i cellens formel. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation/)() | Hämtar alla föregångare (referens till celler i aktuell arbetsbok) som används av cellens formel vid beräkning. |
| [GetRichValue](../../aspose.cells/cell/getrichvalue/)() | Hämtar cellens rika värde. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue/)(CellValueFormatStrategy) | Hämtar strängvärdet med en specifik formateringsstrategi. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle)() | Hämtar cellstilen. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle_1)(bool) | Om checkBorders är true, kontrollera om andra cellers kanter kommer att påverka stilen för den här cellen. |
| [GetTable](../../aspose.cells/cell/gettable/)() | Hämtar tabellen som innehåller den här cellen. |
| [GetValidation](../../aspose.cells/cell/getvalidation/)() | Hämtar valideringen som tillämpas på den här cellen. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue/)() | Hämtar värdet för valideringen som tillämpas på den här cellen. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue/)() | Hämtar bredden på värdet i enheten pixlar. |
| [InsertText](../../aspose.cells/cell/inserttext/)(int, string) | Infoga några tecken i cellen. Om cellen är rik formaterad kan den här metoden behålla den ursprungliga formateringen. |
| [IsRichText](../../aspose.cells/cell/isrichtext/)() | Indikerar om strängvärdet i den här cellen är en rik formaterad text. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue)(bool) | Sätter ett booleskt värde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_3)(DateTime) | Sätter ett DateTime-värde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_1)(double) | Sätter ett double-värde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_2)(int) | Sätter ett heltalsvärde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_4)(object) | Sätter ett objektvärde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_5)(string) | Sätter ett strängvärde i cellen. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_6)(string, bool) | Sätter ett strängvärde i cellen och konverterar värdet till annan datatyp om lämpligt. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_7)(string, bool, bool) | Sätter ett värde i cellen, om lämpligt kommer värdet att konverteras till annan datatyp och cellens talformat återställas. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula/)(bool) | Ta bort matrisformel. |
| [Replace](../../aspose.cells/cell/replace/)(string, string, ReplaceOptions) | Ersätt cellens text med alternativ. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula)(string, int, int) | Ställer in en matrisformel (äldre matrisformel som matas in via CTRL+SHIFT+ENTER i MS Excel) för ett cellområde. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_1)(string, int, int, FormulaParseOptions) | Ställer in en matrisformel för ett cellområde. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Ställer in en matrisformel för ett cellområde. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Ställer in en matrisformel för ett cellområde. |
| [SetCharacters](../../aspose.cells/cell/setcharacters/)(FontSetting[]) | Ställer in rik textformat för cellen. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_2)(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) | Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula)(string, FormulaParseOptions) | Ställ in formeln och värdet (beräknat resultat) för formeln. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_3)(string, object) | Ställ in formeln och värdet (beräknat resultat) för formeln. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_1)(string, FormulaParseOptions, object) | Ställ in formeln och värdet (beräknat resultat) för formeln. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_2)(string, bool, bool, object) | (**Obsolete.**) Ställ in formeln och värdet för formeln. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula)(string, int, int) | Ställer in delade formler för ett cellområde. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_1)(string, int, int, FormulaParseOptions) | Ställer in delade formler för ett cellområde. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Ställer in en formel för ett cellområde. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Ställer in delade formler för ett cellområde. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle)(Style) | Ställer in cellstilen. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_2)(Style, bool) | Applicera den ändrade egenskapen för stilen på cellen. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_1)(Style, StyleFlag) | Applicera cellstilen baserat på flaggor. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_2)(int, int, string, bool, object[][]) | Skapa en envariabels datatabell för det angivna området med start från den här cellen. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_3)(int, int, string, string, object[][]) | Skapa en tvåvariabels datatabell för det angivna området med start från den här cellen. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula)(int, int, int, int, bool, object[][]) | Skapa en envariabels datatabell för det angivna området med start från den här cellen. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_1)(int, int, int, int, int, int, object[][]) | Skapa en tvåvariabels datatabell för det angivna området med start från den här cellen. |
| [ToJson](../../aspose.cells/cell/tojson/)() | Konvertera `Cell` till JSON‑strukturdata. |
| override [ToString](../../aspose.cells/cell/tostring/)() | Returnerar en sträng som representerar det aktuella Cell‑objektet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellDemo
    {
        public static void CellExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            // Åtkomst till cellsamlingen
            Cells cells = worksheet.Cells;

            // Sätt in en sträng i en cell
            Cell cell = cells[0, 0];
            cell.PutValue("Hello");

            // Sätt in ett heltal i en cell
            cell = cells["B1"];
            cell.PutValue(12);

            // Sätt in ett dubbelvärde i en cell
            cell = cells[0, 2];
            cell.PutValue(-1.234);

            // Sätt in en formel i en cell
            cell = cells["D1"];
            cell.Formula = "=B1 + C1";

            // Sätt in en kombinerad formel: "sum(average(b1,c1), b1)" i cellen b2
            cell = cells["B2"];
            cell.Formula = "=sum(average(b1,c1), b1)";

            // Ange stil för en cell
            Style style = cell.GetStyle();
            // Ange bakgrundsfärg
            style.BackgroundColor = System.Drawing.Color.Yellow;
            // Ange teckensnitt för en cell
            style.Font.Name = "Courier New";
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("CellExample.xlsx");
            workbook.Save("CellExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


