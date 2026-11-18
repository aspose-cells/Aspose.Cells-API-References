---
title: "Cell-klass"
linktitle: "Cell"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Cell-klass. Inkapslar objektet som representerar cell i Go."
type: docs
weight: 200
url: /sv/go-cpp/cell/
---

## Cell class

Inkapslar objektet som representerar en enskild arbetsbokscell.

```go

type Cell struct  {
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
| [Calculate](./calculate/) | Beräknar formeln i cellen. |
| [GetWorksheet](./getworksheet/) | Hämtar det överordnade kalkylbladet. |
| [PutValue_Bool](./putvalue_bool/) | Sätter ett booleskt värde i cellen. |
| [PutValue_Int](./putvalue_int/) | Sätter ett heltalsvärde i cellen. |
| [PutValue_Double](./putvalue_double/) | Sätter ett dubbelvärde i cellen. |
| [PutValue_String_Bool_Bool](./putvalue_string_bool_bool/) | Sätter ett värde i cellen, om lämpligt konverteras värdet till en annan datatyp och cellens talformat återställs. |
| [PutValue_String_Bool](./putvalue_string_bool/) | Sätter ett strängvärde i cellen och konverterar värdet till en annan datatyp om lämpligt. |
| [PutValue_String](./putvalue_string/) | Sätter ett strängvärde i cellen. |
| [PutValue_Date](./putvalue_date/) | Sätter ett DateTime‑värde i cellen. |
| [PutValue_Object](./putvalue_object/) | Sätter ett objektvärde i cellen. |
| [GetRow](./getrow/) | Hämtar radnummer (nollbaserat) för cellen. |
| [GetColumn](./getcolumn/) | Hämtar kolumnnummer (nollbaserat) för cellen. |
| [IsFormula](./isformula/) | Anger om den angivna cellen innehåller en formel. |
| [GetHasCustomFunction](./gethascustomfunction/) | Kontrollerar om det finns en anpassad funktion (ej stödd funktion) i cellens formel. |
| [GetType](./gettype/) | Representerar cellens värdetyp. |
| [GetName](./getname/) | Hämtar cellens namn. |
| [IsErrorValue](./iserrorvalue/) | Kontrollerar om värdet i den här cellen är ett fel. |
| [IsNumericValue](./isnumericvalue/) | Indikerar om värdet i den här cellen är numeriskt (int, double och datetime). |
| [GetStringValue_CellValueFormatStrategy](./getstringvalue_cellvalueformatstrategy/) | Hämtar strängvärdet enligt en specifik formateringsstrategi. |
| [GetStringValue](./getstringvalue/) | Hämtar strängvärdet som finns i cellen. Om cellens typ är sträng returneras själva strängvärdet. För andra celltyper returneras det formaterade strängvärdet (formaterat med den angivna stilen för cellen). Det formaterade cellvärdet är detsamma som vad du kan få från Excel när du kopierar en cell som text (t.ex. genom att kopiera cellen till en textredigerare eller exportera till CSV). |
| [GetNumberCategoryType](./getnumbercategorytype/) | Representerar kategoritypen för den här cellens talformatering. |
| [GetDisplayStringValue](./getdisplaystringvalue/) | Hämtar det formaterade strängvärdet för den här cellen enligt cellens visningsstil. |
| [GetIntValue](./getintvalue/) | Hämtar heltalsvärdet som finns i cellen. |
| [GetDoubleValue](./getdoublevalue/) | Hämtar dubbelvärdet som finns i cellen. |
| [GetFloatValue](./getfloatvalue/) | Hämtar flyttalsvärdet som finns i cellen. |
| [GetDateTimeValue](./getdatetimevalue/) | Hämtar DateTime‑värdet som finns i cellen. |
| [GetBoolValue](./getboolvalue/) | Hämtar det booleska värdet som finns i cellen. |
| [GetWidthOfValue](./getwidthofvalue/) | Hämtar bredden på värdet i enheten pixlar. |
| [GetHeightOfValue](./getheightofvalue/) | Hämtar höjden på värdet i enheten pixlar. |
| [GetDisplayStyle](./getdisplaystyle/) | Hämtar visningsstilen för den här cellen. |
| [GetDisplayStyle_Bool](./getdisplaystyle_bool/) | Hämtar visningsstilen för den här cellen. |
| [GetDisplayStyle_BorderType](./getdisplaystyle_bordertype/) | Hämtar visningsstilen för den här cellen. |
| [GetFormatConditions](./getformatconditions/) | Hämtar formatvillkor som gäller för den här cellen. |
| [GetStyle](./getstyle/) | Hämtar cellstilen. |
| [GetStyle_Bool](./getstyle_bool/) | Om checkBorders är sant, kontrollera om andra cellers kanter påverkar stilen för den här cellen. |
| [SetStyle_Style](./setstyle_style/) | Ställer in cellstilen. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Applicera den ändrade stilens egenskap på cellen. |
| [SetStyle_Style_StyleFlag](./setstyle_style_styleflag/) | Applicera cellstilen baserat på flaggor. |
| [GetHasCustomStyle](./gethascustomstyle/) | Anger om den här cellen har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från motsvarande rad, kolumn eller arbetsbok). |
| [GetSharedStyleIndex](./getsharedstyleindex/) | Hämtar cellens delade stilindex i stilpoolen. |
| [GetFormula](./getformula/) | Hämtar eller anger en formel för cellen. |
| [SetFormula_String](./setformula_string/) | Hämtar eller anger en formel för cellen. |
| [GetFormulaLocal](./getformulalocal/) | Hämta den lokalanpassade formeln för cellen. |
| [SetFormulaLocal](./setformulalocal/) | Hämta den lokalanpassade formeln för cellen. |
| [GetR1C1Formula](./getr1c1formula/) | Hämtar eller anger en R1C1-formel för cellen. |
| [SetR1C1Formula](./setr1c1formula/) | Hämtar eller anger en R1C1-formel för cellen. |
| [SetFormula_String_Object](./setformula_string_object/) | Ställ in formeln och värdet (beräknat resultat) för formeln. |
| [SetFormula_String_FormulaParseOptions](./setformula_string_formulaparseoptions/) | Ställ in formeln och värdet (beräknat resultat) för formeln. |
| [GetFormula_Bool_Bool](./getformula_bool_bool/) | Hämta formeln för den här cellen. |
| [SetFormula_String_FormulaParseOptions_Object](./setformula_string_formulaparseoptions_object/) | Ställ in formeln och värdet (beräknat resultat) för formeln. |
| [SetArrayFormula_String_Int_Int](./setarrayformula_string_int_int/) | Ställer in en matrisformel (äldre matrisformel som matas in via CTRL+SHIFT+ENTER i MS Excel) för ett cellområde. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions](./setarrayformula_string_int_int_formulaparseoptions/) | Ställer in en matrisformel för ett cellområde. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setarrayformula_string_int_int_formulaparseoptions_object2array/) | Ställer in en matrisformel för ett cellområde. |
| [SetSharedFormula_String_Int_Int](./setsharedformula_string_int_int/) | Ställer in delade formler för ett cellområde. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions](./setsharedformula_string_int_int_formulaparseoptions/) | Ställer in delade formler för ett cellområde. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setsharedformula_string_int_int_formulaparseoptions_object2array/) | Ställer in delade formler för ett cellområde. |
| [GetContainsExternalLink](./getcontainsexternallink/) | Anger om den här cellen innehåller en extern länk. Gäller endast när cellen är en formelcell. |
| [GetPrecedents](./getprecedents/) | Hämtar alla referenser som förekommer i cellens formel. |
| [GetDependents](./getdependents/) | Hämta alla celler vars formel refererar direkt till den här cellen. |
| [GetPrecedentsInCalculation](./getprecedentsincalculation/) | Hämtar alla föregångare (referenser till celler i aktuell arbetsbok) som används av cellens formel vid beräkning. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Hämtar alla celler vars beräknade resultat beror på den här cellen. |
| [IsArrayHeader](./isarrayheader/) | Indikerar att cellens formel är en matrisformel och att den är den första cellen i matrisen. |
| [IsDynamicArrayFormula](./isdynamicarrayformula/) | Indikerar om cellens formel är en dynamisk matrisformel (true) eller en äldre matrisformel (false). |
| [GetArrayRange](./getarrayrange/) | Hämtar matrisområdet om cellens formel är en matrisformel. |
| [IsArrayFormula](./isarrayformula/) | Indikerar om cellformeln är en matrisformel. |
| [IsSharedFormula](./issharedformula/) | Indikerar om cellformeln är en del av en delad formel. |
| [IsTableFormula](./istableformula/) | Indikerar om den här cellen är en del av en tabellformel. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Bool](./setdynamicarrayformula_string_formulaparseoptions_bool/) | Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool/) | Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool_CalculationOptions](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool_calculationoptions/) | Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt. |
| [SetTableFormula_Int_Int_String_String_Object2Array](./settableformula_int_int_string_string_object2array/) | Skapa en tvåvariabels datatabell för det angivna området med början från den här cellen. |
| [SetTableFormula_Int_Int_String_Bool_Object2Array](./settableformula_int_int_string_bool_object2array/) | Skapa en envariabels datatabell för det angivna området med början från den här cellen. |
| [SetTableFormula_Int_Int_Int_Int_Int_Int_Object2Array](./settableformula_int_int_int_int_int_int_object2array/) | Skapa en tvåvariabels datatabell för det angivna området med början från den här cellen. |
| [SetTableFormula_Int_Int_Int_Int_Bool_Object2Array](./settableformula_int_int_int_int_bool_object2array/) | Skapa en envariabels datatabell för det angivna området med början från den här cellen. |
| [RemoveArrayFormula](./removearrayformula/) | Ta bort matrisformel. |
| [Copy](./copy/) | Kopierar data från en källcell. |
| [GetValue](./getvalue/) | Hämtar/ställer in värdet som finns i den här cellen. |
| [SetValue](./setvalue/) | Hämtar/ställer in värdet som finns i den här cellen. |
| [IsStyleSet](./isstyleset/) | Indikerar om cellens stil är inställd. Om false returneras betyder det att cellen har ett standardformat. |
| [Characters](./characters/) | Returnerar ett Characters-objekt som representerar ett intervall av tecken i cellens text. |
| [Replace](./replace/) | Ersätt cellens text med alternativ. |
| [InsertText](./inserttext/) | Infoga några tecken i cellen. Om cellen har rik formatering kan den här metoden behålla den ursprungliga formateringen. |
| [IsRichText](./isrichtext/) | Indikerar om strängvärdet i den här cellen är rik formaterad text. |
| [GetCharacters](./getcharacters/) | Returnerar alla Characters-objekt som representerar ett intervall av tecken i cellens text. |
| [GetCharacters_Bool](./getcharacters_bool/) | Returnerar alla Characters-objekt som representerar ett intervall av tecken i cellens text. |
| [SetCharacters](./setcharacters/) | Ställer in rik textformat för cellen. |
| [IsMerged](./ismerged/) | Kontrollerar om en cell är en del av ett sammanslaget område eller inte. |
| [GetMergedRange](./getmergedrange/) | Returnerar ett Range-objekt som representerar ett sammanslaget område. |
| [GetComment](./getcomment/) | Hämtar kommentaren för den här cellen. |
| [GetHtmlString](./gethtmlstring/) | Hämtar och ställer in HTML-strängen som innehåller data och vissa format i den här cellen. |
| [SetHtmlString](./sethtmlstring/) | Hämtar och ställer in HTML-strängen som innehåller data och vissa format i den här cellen. |
| [GetHtmlString_Bool](./gethtmlstring_bool/) | Hämtar HTML-strängen som innehåller data och vissa format i den här cellen. |
| [ToString](./tostring/) | Returnerar en sträng som representerar det aktuella Cell‑objektet. |
| [ToJson](./tojson/) | Konvertera cellen till JSON-strukturdatan. |
| [Equals_Object](./equals_object/) | Kontrollerar om detta objekt refererar till samma cell som ett annat. |
| [GetHashCode](./gethashcode/) | Fungerar som en hash-funktion för en viss typ. |
| [Equals_Cell](./equals_cell/) | Kontrollerar om detta objekt refererar till samma cell som ett annat cellobjekt. |
| [GetConditionalFormattingResult](./getconditionalformattingresult/) | Hämta resultatet av den villkorliga formateringen. |
| [GetValidation](./getvalidation/) | Hämtar valideringen som tillämpas på den här cellen. |
| [GetValidationValue](./getvalidationvalue/) | Hämtar värdet av valideringen som tillämpas på den här cellen. |
| [GetTable](./gettable/) | Hämtar tabellen som innehåller den här cellen. |
| [IsCheckBoxStyle](./ischeckboxstyle/) | Anger om den här cellen är inställd som en kryssruta. |
| [SetIsCheckBoxStyle](./setischeckboxstyle/) | Anger om den här cellen är inställd som en kryssruta. |
| [GetRichValue](./getrichvalue/) | Hämtar det rika värdet för cellen. |
| [GetEmbeddedImage](./getembeddedimage/) | Hämtar och anger den inbäddade bilden i cellen. |
| [SetEmbeddedImage](./setembeddedimage/) | Hämtar och anger den inbäddade bilden i cellen. |
| [GetPicture](./getpicture/) | Hämtar en Aspose.Cells.Drawing.Picture-instans för att representera den inbäddade bilden i den här cellen eller null om det inte finns någon inbäddad bild för den här cellen. |
|[Dispose](./dispose/) |  | 
