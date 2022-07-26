---
title: Style
second_title: Aspose.Cells för .NET API-referens
description: Representerar visningsstil för Excel-dokument som typsnitt färg justering kantlinje etc. Stilobjektet innehåller alla stilattribut teckensnitt talformat justering och så vidare som egenskaper.
type: docs
weight: 5750
url: /sv/net/aspose.cells/style/
---
## Style class

Representerar visningsstil för Excel-dokument, som typsnitt, färg, justering, kantlinje, etc. Stilobjektet innehåller alla stilattribut (teckensnitt, talformat, justering och så vidare) som egenskaper.

```csharp
public class Style
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | Hämtar och ställer in bakgrundsfärgen med ett 32-bitars ARGB-värde. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | Hämtar eller ställer in en stils bakgrundsfärg. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | Hämtar och ställer in bakgrundstemafärgen. |
| [Borders](../../aspose.cells/style/borders) { get; } | Får[`BorderCollection`](../bordercollection) av stilen. |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | Hämtar och ställer in den kulturberoende mönstersträngen för talformat. Om inget talformat har ställts in för detta objekt kommer null att returneras. Om talformat är inbyggt kommer mönstersträngen som motsvarar det inbyggda numret att returneras. |
| [Custom](../../aspose.cells/style/custom) { get; set; } | Representerar den anpassade talformatsträngen för det här stilobjektet. Om det anpassade talformatet inte är inställt (t.ex. talformatet är inbyggt), kommer "" att returneras. |
| [Font](../../aspose.cells/style/font) { get; } | Får en[`Font`](./font) objekt. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | Hämtar och ställer in förgrundsfärgen med ett 32-bitars ARGB-värde. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | Hämtar eller ställer in en stils förgrundsfärg. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | Hämtar och ställer in förgrundstemafärgen. |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | Kontrollerar om det finns gränser har ställts in för stilen. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | Hämtar eller ställer in den horisontella anpassningstypen för texten i en cell. |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | Representerar indragsnivån för cellen eller området. Kan bara vara ett heltal från 0 till 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | Hämtar den kulturoberoende mönstersträngen för talformat. Om inget talformat har ställts in för detta objekt returneras null. Om talformat är inbyggt returneras mönstersträngen som motsvarar det inbyggda numret. |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | Indikerar om talformatet är ett datumformat. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | Representerar om formeln kommer att döljas när kalkylbladet är skyddat. |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | Indikerar om cellskuggningen är ett gradientmönster. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | Indikerar om cellerna justerad eller distribuerad justering ska användas på den sista textraden. |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | Hämtar eller ställer in ett värde som anger om en cell kan ändras eller inte. |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | Indikerar om talformatet är ett procentformat. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | Hämtar eller ställer in ett värde som anger om texten i en cell är radbruten. |
| [Name](../../aspose.cells/style/name) { get; set; } | Hämtar eller ställer in namnet på stilen. |
| [Number](../../aspose.cells/style/number) { get; set; } | Hämtar eller ställer in visningsformatet för siffror och datum. Formateringsmönstren är olika för olika regioner. |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | Hämtar den överordnade stilen för denna stil. |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | Hämtar eller ställer in cellbakgrundsmönstertypen. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | Indikerar om cellens värde börjar med enkla citattecken. |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | Representerar textrotationsvinkel. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | Representerar om text automatiskt krymper för att passa den tillgängliga kolumnbredden. |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | Representerar textläsordning. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | Hämtar eller ställer in den vertikala anpassningstypen för texten i en cell. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | Kopierar data från ett annat stilobjekt |
| override [Equals](../../aspose.cells/style/equals)(object) | Bestämmer om två stilinstanser är lika. |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | Fungerar som en hashfunktion för ett Style-objekt. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | Hämta tvåfärgsgradientinställningen. |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | Kontrollerar om de angivna egenskaperna för stilen har ändrats. Används för stil för ConditionalFormattings för att kontrollera om de angivna egenskaperna för denna stil ska användas när de ConditionalFormattings tillämpas på en cell. |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | Ställer in gränserna för stilen. |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | Ställer in den anpassade talformatsträngen för en cell. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | Ställer in bakgrundsfärgen. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgsgradient. |
| [Update](../../aspose.cells/style/update)() | Tillämpa den namngivna stilen på stilarna i cellerna som använder den här namngivna stilen. Det fungerar som att klicka på "ok"-knappen efter att du avslutat modifieringen av stilen. Gäller endast för namngiven stil. |

### Exempel

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
