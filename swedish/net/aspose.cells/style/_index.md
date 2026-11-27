---
title: "Klass Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Style‑klass. Representerar visningsstil för Excel‑dokument såsom teckensnitt, färg, justering, kant osv. Style‑objektet innehåller alla stilattribut som teckensnitt, talformat, justering och så vidare som egenskaper"
type: docs
url: /sv/net/aspose.cells/style/
---
## Style class

Representerar visningsstilen för Excel‑dokument, såsom teckensnitt, färg, justering, kantlinje osv. Style‑objektet innehåller alla stilattribut (teckensnitt, talformat, justering osv.) som egenskaper.

```csharp
public class Style
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Style](style/)() | (**Obsolete.**) Initierar en ny instans av `Style`‑klassen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor/) { get; set; } | Hämtar och anger bakgrundsfärgen med ett 32‑bitars ARGB‑värde. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor/) { get; set; } | Hämtar eller anger en stils bakgrundsfärg. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor/) { get; set; } | Hämtar och anger bakgrundens temafärg. |
| [Borders](../../aspose.cells/style/borders/) { get; } | Hämtar [`BorderCollection`](../bordercollection/) för stilen. |
| [BottomBorder](../../aspose.cells/style/bottomborder/) { get; } | Hämtar den nedre kanten. |
| [CultureCustom](../../aspose.cells/style/culturecustom/) { get; set; } | Hämtar och anger det kulturspecifika mönstersträngen för talformat. Om inget talformat har angetts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet. |
| [Custom](../../aspose.cells/style/custom/) { get; set; } | Representerar den anpassade talformatsträngen för detta stilobjekt. Om det anpassade talformatet inte är angivet (till exempel om talformatet är inbyggt) returneras "". |
| [Font](../../aspose.cells/style/font/) { get; } | Hämtar ett [`Font`](./font/) objekt. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor/) { get; set; } | Hämtar och anger förgrundsfärgen med ett 32‑bitars ARGB‑värde. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor/) { get; set; } | Hämtar eller anger en stils förgrundsfärg. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor/) { get; set; } | Hämtar och anger förgrundens temafärg. |
| [HasBorders](../../aspose.cells/style/hasborders/) { get; } | Kontrollerar om det finns kanter som har satts för stilen. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment/) { get; set; } | Hämtar eller anger den horisontella justeringstypen för texten i en cell. |
| [IndentLevel](../../aspose.cells/style/indentlevel/) { get; set; } | Representerar indenteringsnivån för cellen eller området. Kan endast vara ett heltal mellan 0 och 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom/) { get; } | Hämtar det kulturoberoende mönsterssträngen för talformat. Om inget talformat har satts för detta objekt returneras null. Om talformatet är inbyggt returneras mönsterssträngen som motsvarar det inbyggda talet. |
| [IsAlignmentApplied](../../aspose.cells/style/isalignmentapplied/) { get; set; } | Anger om justeringsformateringen ska tillämpas. |
| [IsBorderApplied](../../aspose.cells/style/isborderapplied/) { get; set; } | Anger om kantformateringen ska tillämpas. |
| [IsCheckBox](../../aspose.cells/style/ischeckbox/) { get; set; } | Anger om det är en stil för kryssruta. |
| [IsDateTime](../../aspose.cells/style/isdatetime/) { get; } | Anger om talformatet är ett datumformat. |
| [IsFillApplied](../../aspose.cells/style/isfillapplied/) { get; set; } | Anger om fyllnadsformateringen ska tillämpas. |
| [IsFontApplied](../../aspose.cells/style/isfontapplied/) { get; set; } | Anger om teckensnittsformateringen ska tillämpas. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden/) { get; set; } | Representerar om formeln kommer att döljas när kalkylbladet är skyddat. |
| [IsGradient](../../aspose.cells/style/isgradient/) { get; set; } | Anger om cellskuggning är ett gradientmönster. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed/) { get; set; } | Anger om cellerna ska ha justerad eller fördelad justering på den sista textraden. |
| [IsLocked](../../aspose.cells/style/islocked/) { get; set; } | Hämtar eller anger ett värde som indikerar om en cell kan ändras eller inte. |
| [IsNumberFormatApplied](../../aspose.cells/style/isnumberformatapplied/) { get; set; } | Anger om talformateringen ska tillämpas. |
| [IsPercent](../../aspose.cells/style/ispercent/) { get; } | Anger om talformatet är ett procentformat. |
| [IsProtectionApplied](../../aspose.cells/style/isprotectionapplied/) { get; set; } | Anger om skyddsformateringen ska tillämpas. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped/) { get; set; } | Hämtar eller anger ett värde som indikerar om texten i en cell är radbruten. |
| [LeftBorder](../../aspose.cells/style/leftborder/) { get; } | Hämtar vänsterkanten. |
| [Name](../../aspose.cells/style/name/) { get; set; } | Hämtar eller anger stilens namn. |
| [Number](../../aspose.cells/style/number/) { get; set; } | Hämtar eller anger visningsformatet för tal och datum. Formateringsmönstren skiljer sig åt mellan olika regioner. |
| [ParentStyle](../../aspose.cells/style/parentstyle/) { get; } | Hämtar den överordnade stilen för denna stil. |
| [Pattern](../../aspose.cells/style/pattern/) { get; set; } | Hämtar eller anger cellens bakgrundsmönstertyp. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix/) { get; set; } | Indikerar om cellens värde börjar med enkelfnutt. |
| [RightBorder](../../aspose.cells/style/rightborder/) { get; } | Hämtar den högra kanten. |
| [RotationAngle](../../aspose.cells/style/rotationangle/) { get; set; } | Representerar textrotationsvinkeln. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit/) { get; set; } | Representerar om text automatiskt krymper för att passa i den tillgängliga kolumnbredden. |
| [TextDirection](../../aspose.cells/style/textdirection/) { get; set; } | Representerar textens läsriktning. |
| [TopBorder](../../aspose.cells/style/topborder/) { get; } | Hämtar den övre kanten. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment/) { get; set; } | Hämtar eller anger den vertikala justeringstypen för texten i en cell. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Copy](../../aspose.cells/style/copy/)(Style) | Kopierar data från ett annat stilobjekt |
| override [Equals](../../aspose.cells/style/equals/)(object) | Bestämmer om två Style-instanser är lika. |
| override [GetHashCode](../../aspose.cells/style/gethashcode/)() | Fungerar som en hashfunktion för ett Style-objekt. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient/)(out Color, out Color, out GradientStyleType, out int) | (**Obsolete.**) Hämta den tvåfärgade gradientinställningen. |
| [GetTwoColorGradientSetting](../../aspose.cells/style/gettwocolorgradientsetting/)() | Hämta den tvåfärgade gradientinställningen. |
| [IsModified](../../aspose.cells/style/ismodified/)(StyleModifyFlag) | Kontrollerar om de angivna egenskaperna för stilen har ändrats. Används för stil av ConditionalFormattings för att kontrollera om de angivna egenskaperna för denna stil ska användas när ConditionalFormattings tillämpas på en cell. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder)(BorderType, CellBorderType, CellsColor) | Ställer in kanterna för stilen. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder_1)(BorderType, CellBorderType, Color) | Ställer in kanterna för stilen. |
| [SetCustom](../../aspose.cells/style/setcustom/)(string, bool) | Ställer in den anpassade talformatsträngen för en cell. |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Ställ in konturkanterna |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Ställ in konturkanterna |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor/)(BackgroundType, Color, Color) | Ställer in bakgrundsfärgen. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient/)(Color, Color, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgad gradient. |
| [ToJson](../../aspose.cells/style/tojson/)() | Konvertera `Style` till JSON‑strukturdata. |
| [Update](../../aspose.cells/style/update/)() | Applicera den namngivna stilen på stilarna för de celler som använder denna namngivna stil. Det fungerar som att klicka på "ok"‑knappen efter att du har avslutat att modifiera stilen. Gäller endast för namngivna stilar. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleDemo
    {
        public static void StyleExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till en cell från kalkylbladet
            Cell cell = worksheet.Cells["A1"];
            
            // Hämta stil för cellen
            Style style = cell.GetStyle();
            
            // Ställ in olika egenskaper för stilen
            style.Font.Name = "Times New Roman";
            style.Font.Color = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;
            style.IsLocked = true;
            style.Number = 15; // Date format
            style.IndentLevel = 2;
            style.RotationAngle = 45;
            style.IsFormulaHidden = true;
            style.ShrinkToFit = true;
            style.TextDirection = TextDirectionType.RightToLeft;
            style.IsJustifyDistributed = true;
            style.QuotePrefix = true;
            style.IsGradient = true;
            style.IsNumberFormatApplied = true;
            style.IsFontApplied = true;
            style.IsAlignmentApplied = true;
            style.IsBorderApplied = true;
            style.IsFillApplied = true;
            style.IsProtectionApplied = true;
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.ForegroundArgbColor = Color.Red.ToArgb();
            style.Custom = "0.00%";
            style.CultureCustom = "0.00%";
            
            // Ställ in stilen på cellen
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("StyleExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


