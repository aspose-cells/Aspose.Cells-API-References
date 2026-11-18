---
title: "Style klass"
linktitle: "Style"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Style klass. Inkapslar objektet som representerar style i Go."
type: docs
weight: 200
url: /sv/go-cpp/style/
---

## Style class

Representerar visningsstilen för Excel-dokument, såsom teckensnitt, färg, justering, kantlinje osv. Style-objektet innehåller alla stilattribut (teckensnitt, talformat, justering med mera) som egenskaper.

```go

type Style struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetBackgroundThemeColor](./getbackgroundthemecolor/) | Hämtar och anger bakgrundstemat färg. |
| [SetBackgroundThemeColor](./setbackgroundthemecolor/) | Hämtar och anger bakgrundstemat färg. |
| [GetForegroundThemeColor](./getforegroundthemecolor/) | Hämtar och anger förgrundstemat färg. |
| [SetForegroundThemeColor](./setforegroundthemecolor/) | Hämtar och anger förgrundstemat färg. |
| [GetName](./getname/) | Hämtar eller anger namnet på stilen. |
| [SetName](./setname/) | Hämtar eller anger namnet på stilen. |
| [GetPattern](./getpattern/) | Hämtar eller anger cellens bakgrundsmönstertyp. |
| [SetPattern](./setpattern/) | Hämtar eller anger cellens bakgrundsmönstertyp. |
| [SetPatternColor](./setpatterncolor/) | Anger bakgrundsfärgen. |
| [GetBorders](./getborders/) | Hämtar BorderCollection för stilen. |
| [GetBackgroundColor](./getbackgroundcolor/) | Hämtar eller anger en stils bakgrundsfärg. |
| [SetBackgroundColor](./setbackgroundcolor/) | Hämtar eller anger en stils bakgrundsfärg. |
| [GetBackgroundArgbColor](./getbackgroundargbcolor/) | Hämtar och anger bakgrundsfärgen med ett 32-bitars ARGB‑värde. |
| [SetBackgroundArgbColor](./setbackgroundargbcolor/) | Hämtar och anger bakgrundsfärgen med ett 32-bitars ARGB‑värde. |
| [GetForegroundColor](./getforegroundcolor/) | Hämtar eller anger en stils förgrundsfärg. |
| [SetForegroundColor](./setforegroundcolor/) | Hämtar eller anger en stils förgrundsfärg. |
| [GetForegroundArgbColor](./getforegroundargbcolor/) | Hämtar och anger förgrundsfärgen med ett 32-bitars ARGB‑värde. |
| [SetForegroundArgbColor](./setforegroundargbcolor/) | Hämtar och anger förgrundsfärgen med ett 32-bitars ARGB‑värde. |
| [Copy](./copy/) | Kopierar data från ett annat style‑objekt |
| [GetHasBorders](./gethasborders/) | Kontrollerar om det finns kanter som har satts för stilen. |
| [GetParentStyle](./getparentstyle/) | Hämtar föräldrastilen för denna stil. |
| [Update](./update/) | Applicera den namngivna stilen på cellernas stilar som använder denna namngivna stil. Det fungerar som att klicka på "ok"-knappen efter att du har avslutat modifieringen av stilen. Gäller endast för namngivna stilar. |
| [IsNumberFormatApplied](./isnumberformatapplied/) | Indikera om talformatering ska tillämpas. |
| [SetIsNumberFormatApplied](./setisnumberformatapplied/) | Indikera om talformatering ska tillämpas. |
| [IsFontApplied](./isfontapplied/) | Ange om teckensnittsformatering ska tillämpas. |
| [SetIsFontApplied](./setisfontapplied/) | Ange om teckensnittsformatering ska tillämpas. |
| [IsAlignmentApplied](./isalignmentapplied/) | Ange om justeringsformatering ska tillämpas. |
| [SetIsAlignmentApplied](./setisalignmentapplied/) | Ange om justeringsformatering ska tillämpas. |
| [IsBorderApplied](./isborderapplied/) | Ange om kantformatering ska tillämpas. |
| [SetIsBorderApplied](./setisborderapplied/) | Ange om kantformatering ska tillämpas. |
| [IsFillApplied](./isfillapplied/) | Ange om fyllningsformatering ska tillämpas. |
| [SetIsFillApplied](./setisfillapplied/) | Ange om fyllningsformatering ska tillämpas. |
| [IsProtectionApplied](./isprotectionapplied/) | Ange om skyddsformatering ska tillämpas. |
| [SetIsProtectionApplied](./setisprotectionapplied/) | Ange om skyddsformatering ska tillämpas. |
| [IsModified](./ismodified/) | Kontrollerar om de angivna egenskaperna för stilen har ändrats. Används för stil av ConditionalFormattings för att kontrollera om de angivna egenskaperna för denna stil ska användas när ConditionalFormattings tillämpas på en cell. |
| [Equals](./equals/) | Bestämmer om två Style-instans är lika. |
| [GetHashCode](./gethashcode/) | Fungerar som en hashfunktion för ett Style-objekt. |
| [GetIndentLevel](./getindentlevel/) | Representerar indenteringsnivån för cellen eller området. Kan endast vara ett heltal mellan 0 och 250. |
| [SetIndentLevel](./setindentlevel/) | Representerar indenteringsnivån för cellen eller området. Kan endast vara ett heltal mellan 0 och 250. |
| [GetFont](./getfont/) | Hämtar ett Font-objekt. |
| [GetRotationAngle](./getrotationangle/) | Representerar textrotationsvinkel. |
| [SetRotationAngle](./setrotationangle/) | Representerar textrotationsvinkel. |
| [GetHorizontalAlignment](./gethorizontalalignment/) | Hämtar eller anger den horisontella justeringstypen för texten i en cell. |
| [SetHorizontalAlignment](./sethorizontalalignment/) | Hämtar eller anger den horisontella justeringstypen för texten i en cell. |
| [GetVerticalAlignment](./getverticalalignment/) | Hämtar eller anger den vertikala justeringstypen för texten i en cell. |
| [SetVerticalAlignment](./setverticalalignment/) | Hämtar eller anger den vertikala justeringstypen för texten i en cell. |
| [IsTextWrapped](./istextwrapped/) | Hämtar eller anger ett värde som indikerar om texten i en cell är radbruten. |
| [SetIsTextWrapped](./setistextwrapped/) | Hämtar eller anger ett värde som indikerar om texten i en cell är radbruten. |
| [GetNumber](./getnumber/) | Hämtar eller anger visningsformatet för tal och datum. Formateringsmönstren är olika för olika regioner. |
| [SetNumber](./setnumber/) | Hämtar eller anger visningsformatet för tal och datum. Formateringsmönstren är olika för olika regioner. |
| [SetBorder_BorderType_CellBorderType_Color](./setborder_bordertype_cellbordertype_color/) | Anger kantlinjerna för stilen. |
| [SetBorder_BorderType_CellBorderType_CellsColor](./setborder_bordertype_cellbordertype_cellscolor/) | Anger kantlinjerna för stilen. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Ange konturkanterna |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Ange konturkanterna |
| [IsLocked](./islocked/) | Hämtar eller anger ett värde som indikerar om en cell kan modifieras eller inte. |
| [SetIsLocked](./setislocked/) | Hämtar eller anger ett värde som indikerar om en cell kan modifieras eller inte. |
| [SetCustom_String_Bool](./setcustom_string_bool/) | Anger den anpassade talformatsträngen för en cell. |
| [GetCustom](./getcustom/) | Representerar den anpassade talformatsträngen för detta stilobjekt. Om den anpassade talformatet inte är inställt (till exempel om talformatet är inbyggt) returneras "". |
| [SetCustom_String](./setcustom_string/) | Representerar den anpassade talformatsträngen för detta stilobjekt. Om den anpassade talformatet inte är inställt (till exempel om talformatet är inbyggt) returneras "". |
| [GetCultureCustom](./getculturecustom/) | Hämtar och anger det kulturberoende mönstersträngen för talformat. Om inget talformat har angetts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet. |
| [SetCultureCustom](./setculturecustom/) | Hämtar och anger det kulturberoende mönstersträngen för talformat. Om inget talformat har angetts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet. |
| [GetInvariantCustom](./getinvariantcustom/) | Hämtar den kulturoberoende mönstersträngen för talformat. Om inget talformat har angetts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet. |
| [IsFormulaHidden](./isformulahidden/) | Representerar om formeln ska döljas när arbetsbladet är skyddat. |
| [SetIsFormulaHidden](./setisformulahidden/) | Representerar om formeln ska döljas när arbetsbladet är skyddat. |
| [GetShrinkToFit](./getshrinktofit/) | Representerar om text automatiskt krymper för att passa den tillgängliga kolumnbredden. |
| [SetShrinkToFit](./setshrinktofit/) | Representerar om text automatiskt krymper för att passa den tillgängliga kolumnbredden. |
| [GetTextDirection](./gettextdirection/) | Representerar läsordning för text. |
| [SetTextDirection](./settextdirection/) | Representerar läsordning för text. |
| [IsJustifyDistributed](./isjustifydistributed/) | Indikerar om cellernas justerade eller fördelade justering ska användas på den sista textraden. |
| [SetIsJustifyDistributed](./setisjustifydistributed/) | Indikerar om cellernas justerade eller fördelade justering ska användas på den sista textraden. |
| [GetQuotePrefix](./getquoteprefix/) | Anger om cellens värde börjar med ett enkelt citattecken. |
| [SetQuotePrefix](./setquoteprefix/) | Anger om cellens värde börjar med ett enkelt citattecken. |
| [IsGradient](./isgradient/) | Anger om cellskuggning är ett gradientmönster. |
| [SetIsGradient](./setisgradient/) | Anger om cellskuggning är ett gradientmönster. |
| [SetTwoColorGradient](./settwocolorgradient/) | Ställer in den angivna fyllningen till en tvåfärgsgradient. |
| [GetTwoColorGradientSetting](./gettwocolorgradientsetting/) | Hämta inställningen för tvåfärgsgradient. |
| [IsPercent](./ispercent/) | Anger om talformatet är ett procentformat. |
| [IsDateTime](./isdatetime/) | Anger om talformatet är ett datumformat. |
| [IsCheckBox](./ischeckbox/) | Anger om det är en stil för kryssruta. |
| [SetIsCheckBox](./setischeckbox/) | Anger om det är en stil för kryssruta. |
| [ToJson](./tojson/) | Konvertera stil till JSON-strukturdata. |
| [GetLeftBorder](./getleftborder/) | Hämtar den vänstra kanten. |
| [GetRightBorder](./getrightborder/) | Hämtar den högra kanten. |
| [GetTopBorder](./gettopborder/) | Hämtar den övre kanten. |
| [GetBottomBorder](./getbottomborder/) | Hämtar den nedre kanten. |
