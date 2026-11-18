---
title: "RectangleShape-klass"
linktitle: "RectangleShape"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "RectangleShape-klass. Inkapslar objektet som representerar rectangleshape i Go."
type: docs
weight: 200
url: /sv/go-cpp/rectangleshape/
---

## RectangleShape class

Representerar rektangelformen.

```go

type RectangleShape struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewRectangleShape](./newrectangleshape/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetMacroName](./getmacroname/) | Hämtar och anger namnet på makrot. |
| [SetMacroName](./setmacroname/) | Hämtar och anger namnet på makrot. |
| [IsEquation](./isequation/) | Anger om formen endast innehåller en ekvation. |
| [IsSmartArt](./issmartart/) | Anger om formen är en smart art. |
| [ToFrontOrBack](./tofrontorback/) | Flyttar formen till framgrunden eller skickar formen till bakgrunden. |
| [GetZOrderPosition](./getzorderposition/) | Returnerar positionen för en form i z-ordningen. |
| [SetZOrderPosition](./setzorderposition/) | Returnerar positionen för en form i z-ordningen. |
| [GetName](./getname/) | Hämtar och anger namnet på formen. |
| [SetName](./setname/) | Hämtar och anger namnet på formen. |
| [GetAlternativeText](./getalternativetext/) | Returnerar eller anger den beskrivande (alternativa) textsträngen för Shape-objektet. |
| [SetAlternativeText](./setalternativetext/) | Returnerar eller anger den beskrivande (alternativa) textsträngen för Shape-objektet. |
| [GetTitle](./gettitle/) | Anger titeln (rubriken) för det aktuella shape-objektet. |
| [SetTitle](./settitle/) | Anger titeln (rubriken) för det aktuella shape-objektet. |
| [GetLine](./getline/) | Hämtar linjestil |
| [GetFill](./getfill/) | Returnerar ett FillFormat-objekt som innehåller fyllningsformaterings‑egenskaper för den angivna formen. |
| [GetShadowEffect](./getshadoweffect/) | Representerar ett Drawing.ShadowEffect-objekt som specificerar skuggeffekt för diagram‑elementet eller formen. |
| [GetReflection](./getreflection/) | Representerar ett ReflectionEffect-objekt som specificerar reflektionseffekt för diagram‑elementet eller formen. |
| [GetGlow](./getglow/) | Representerar ett GlowEffect-objekt som specificerar glödeffekt för diagram‑elementet eller formen. |
| [GetSoftEdges](./getsoftedges/) | Hämtar och anger radien för suddighet som ska tillämpas på kanterna, i enheten punkter. |
| [SetSoftEdges](./setsoftedges/) | Hämtar och anger radien för suddighet som ska tillämpas på kanterna, i enheten punkter. |
| [GetThreeDFormat](./getthreedformat/) | Hämtar och anger 3D-formatet för formen. |
| [GetFormatPicture](./getformatpicture/) | Hämtar och anger alternativen för bildformatet. |
| [IsHidden](./ishidden/) | Anger om objektet är synligt. |
| [SetIsHidden](./setishidden/) | Anger om objektet är synligt. |
| [IsAspectRatioLocked](./isaspectratiolocked/) | Sant betyder att bildförhållandet för formen är låst. |
| [SetIsAspectRatioLocked](./setisaspectratiolocked/) | Sant betyder att bildförhållandet för formen är låst. |
| [GetLockedProperty](./getlockedproperty/) | Hämtar värdet för låst‑egenskapen. |
| [SetLockedProperty](./setlockedproperty/) | Ange den låsta egenskapen. |
| [GetRotationAngle](./getrotationangle/) | Hämtar och anger rotationen för formen. |
| [SetRotationAngle](./setrotationangle/) | Hämtar och anger rotationen för formen. |
| [AddHyperlink](./addhyperlink/) | Lägger till en hyperlänk till formen. |
| [RemoveHyperlink](./removehyperlink/) | Tar bort hyperlänken för formen. |
| [GetHyperlink](./gethyperlink/) | Hämtar hyperlänken för formen. |
| [MoveToRange](./movetorange/) | Flyttar formen till ett angivet område. |
| [AlignTopRightCorner](./aligntoprightcorner/) | Flyttar bilden till det övre högra hörnet. |
| [GetId](./getid/) | Hämtar identifieraren för denna form. |
| [GetSpid](./getspid/) | Anger en valfri strängidentifierare som en applikation kan använda för att identifiera den specifika formen. |
| [GetSpt](./getspt/) | Anger ett valfritt nummer som en applikation kan använda för att associera den specifika formen med en definierad formtyp. |
| [GetWorksheet](./getworksheet/) | Hämtar Aspose.Cells.Worksheet-objektet som innehåller den här formen. |
| [IsGroup](./isgroup/) | Anger om den här formen är en gruppform. |
| [IsInGroup](./isingroup/) | Anger om formen är grupperad. |
| [IsWordArt](./iswordart/) | Anger om den här formen är en WordArt. |
| [GetTextEffect](./gettexteffect/) | Returnerar ett TextEffectFormat-objekt som innehåller text‑effektformateringsegenskaper för den angivna formen. Gäller Shape-objekt som representerar WordArt. |
| [IsLocked](./islocked/) | True betyder att objektet inte kan modifieras när bladet är skyddat. Observera att detta värde endast är meningsfullt om arbetsbladet eller objekt i arbetsbladet är skyddade. |
| [SetIsLocked](./setislocked/) | True betyder att objektet inte kan modifieras när bladet är skyddat. Observera att detta värde endast är meningsfullt om arbetsbladet eller objekt i arbetsbladet är skyddade. |
| [IsPrintable](./isprintable/) | Anger om objektet är utskrivbart. Om False kommer denna form inte att skrivas ut vid utskrift. |
| [SetIsPrintable](./setisprintable/) | Anger om objektet är utskrivbart. Om False kommer denna form inte att skrivas ut vid utskrift. |
| [GetMsoDrawingType](./getmsodrawingtype/) | Hämtar ritningstyp. |
| [GetAutoShapeType](./getautoshapetype/) | Hämtar och anger autoformtypen. |
| [SetAutoShapeType](./setautoshapetype/) | Hämtar och anger autoformtypen. |
| [GetAnchorType](./getanchortype/) | Hämtar och anger typen av formens ankare‑platshållare. |
| [SetAnchorType](./setanchortype/) | Hämtar och anger typen av formens ankare‑platshållare. |
| [GetPlacement](./getplacement/) | Representerar hur ritningsobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett arbetsblad. |
| [SetPlacement](./setplacement/) | Representerar hur ritningsobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett arbetsblad. |
| [GetUpperLeftRow](./getupperleftrow/) | Representerar index för översta raden. |
| [SetUpperLeftRow](./setupperleftrow/) | Representerar index för översta raden. |
| [GetUpperDeltaY](./getupperdeltay/) | Hämtar eller anger formens vertikala förskjutning från dess övre vänstra hörnrad. |
| [SetUpperDeltaY](./setupperdeltay/) | Hämtar eller anger formens vertikala förskjutning från dess övre vänstra hörnrad. |
| [GetUpperLeftColumn](./getupperleftcolumn/) | Representerar index för övre vänstra hörnkolumn. |
| [SetUpperLeftColumn](./setupperleftcolumn/) | Representerar index för övre vänstra hörnkolumn. |
| [GetUpperDeltaX](./getupperdeltax/) | Hämtar eller anger formens horisontella förskjutning från dess övre vänstra hörnkolumn. |
| [SetUpperDeltaX](./setupperdeltax/) | Hämtar eller anger formens horisontella förskjutning från dess övre vänstra hörnkolumn. |
| [GetLowerRightRow](./getlowerrightrow/) | Representerar index för nedre högra hörnrad. |
| [SetLowerRightRow](./setlowerrightrow/) | Representerar index för nedre högra hörnrad. |
| [GetLowerDeltaY](./getlowerdeltay/) | Hämtar eller anger formens vertikala förskjutning från dess nedre högra hörnrad. |
| [SetLowerDeltaY](./setlowerdeltay/) | Hämtar eller anger formens vertikala förskjutning från dess nedre högra hörnrad. |
| [GetLowerRightColumn](./getlowerrightcolumn/) | Representerar index för nedre högra hörnkolumn. |
| [SetLowerRightColumn](./setlowerrightcolumn/) | Representerar index för nedre högra hörnkolumn. |
| [GetLowerDeltaX](./getlowerdeltax/) | Hämtar eller anger formens horisontella förskjutning från dess nedre högra hörnkolumn. |
| [SetLowerDeltaX](./setlowerdeltax/) | Hämtar eller anger formens horisontella förskjutning från dess nedre högra hörnkolumn. |
| [GetRight](./getright/) | Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enheten pixlar. |
| [SetRight](./setright/) | Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enheten pixlar. |
| [GetBottom](./getbottom/) | Representerar bredden på formens vertikala förskjutning från dess nedre bottenhörnrad, i enheten pixlar. |
| [SetBottom](./setbottom/) | Representerar bredden på formens vertikala förskjutning från dess nedre bottenhörnrad, i enheten pixlar. |
| [GetWidth](./getwidth/) | Representerar formens bredd, i enheten pixlar. |
| [SetWidth](./setwidth/) | Representerar formens bredd, i enheten pixlar. |
| [GetWidthInch](./getwidthinch/) | Representerar formens bredd, i enheten tum. |
| [SetWidthInch](./setwidthinch/) | Representerar formens bredd, i enheten tum. |
| [GetWidthPt](./getwidthpt/) | Representerar formens bredd, i enheten punkt. |
| [SetWidthPt](./setwidthpt/) | Representerar formens bredd, i enheten punkt. |
| [GetWidthCM](./getwidthcm/) | Representerar formens bredd, i enheten centimeter. |
| [SetWidthCM](./setwidthcm/) | Representerar formens bredd, i enheten centimeter. |
| [GetHeight](./getheight/) | Representerar höjden på formen, i enhet pixel. |
| [SetHeight](./setheight/) | Representerar höjden på formen, i enhet pixel. |
| [GetHeightInch](./getheightinch/) | Representerar höjden på formen, i enhet tum. |
| [SetHeightInch](./setheightinch/) | Representerar höjden på formen, i enhet tum. |
| [GetHeightPt](./getheightpt/) | Representerar höjden på formen, i enhet punkter. |
| [SetHeightPt](./setheightpt/) | Representerar höjden på formen, i enhet punkter. |
| [GetHeightCM](./getheightcm/) | Representerar höjden på formen, i enhet centimeter. |
| [SetHeightCM](./setheightcm/) | Representerar höjden på formen, i enhet centimeter. |
| [GetLeft](./getleft/) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar. |
| [SetLeft](./setleft/) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar. |
| [GetLeftInch](./getleftinch/) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet tum. |
| [SetLeftInch](./setleftinch/) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet tum. |
| [GetLeftCM](./getleftcm/) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet centimeter. |
| [SetLeftCM](./setleftcm/) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet centimeter. |
| [GetTop](./gettop/) | Representerar den vertikala förskjutningen av formen från dess översta rad, i enhet pixlar. |
| [SetTop](./settop/) | Representerar den vertikala förskjutningen av formen från dess översta rad, i enhet pixlar. |
| [GetTopInch](./gettopinch/) | Representerar den vertikala förskjutningen av formen från dess översta rad, i enhet tum. |
| [SetTopInch](./settopinch/) | Representerar den vertikala förskjutningen av formen från dess översta rad, i enhet tum. |
| [GetTopCM](./gettopcm/) | Representerar den vertikala förskjutningen av formen från dess översta rad, i enhet centimeter. |
| [SetTopCM](./settopcm/) | Representerar den vertikala förskjutningen av formen från dess översta rad, i enhet centimeter. |
| [GetTopToCorner](./gettoptocorner/) | Hämtar och anger den vertikala förskjutningen av formen från kalkylbladets övre kant, i enhet pixlar. |
| [SetTopToCorner](./settoptocorner/) | Hämtar och anger den vertikala förskjutningen av formen från kalkylbladets övre kant, i enhet pixlar. |
| [GetLeftToCorner](./getlefttocorner/) | Hämtar och anger den horisontella förskjutningen av formen från kalkylbladets vänstra kant. |
| [SetLeftToCorner](./setlefttocorner/) | Hämtar och anger den horisontella förskjutningen av formen från kalkylbladets vänstra kant. |
| [GetX](./getx/) | Hämtar och anger den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enhet pixlar. |
| [SetX](./setx/) | Hämtar och anger den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enhet pixlar. |
| [GetY](./gety/) | Hämtar och anger den vertikala förskjutningen av formen från kalkylbladets övre kant, i enhet pixlar. |
| [SetY](./sety/) | Hämtar och anger den vertikala förskjutningen av formen från kalkylbladets övre kant, i enhet pixlar. |
| [GetWidthScale](./getwidthscale/) | Hämtar och anger breddskalan, i enhet procent av den ursprungliga bildens bredd. Om formen inte är en bild, returnerar WidthScale property endast 100; |
| [SetWidthScale](./setwidthscale/) | Hämtar och anger breddskalan, i enhet procent av den ursprungliga bildens bredd. Om formen inte är en bild, returnerar WidthScale property endast 100; |
| [GetHeightScale](./getheightscale/) | Hämtar och anger höjds skalan, i enhet procent av den ursprungliga bildens höjd. Om formen inte är en bild, returnerar HeightScale property endast 100; |
| [SetHeightScale](./setheightscale/) | Hämtar och anger höjds skalan, i enhet procent av den ursprungliga bildens höjd. Om formen inte är en bild, returnerar HeightScale property endast 100; |
| [GetTopInShape](./gettopinshape/) | Representerar den vertikala förskjutningen av formen från den översta kanten av föräldraformen, i enhet 1/4000 av föräldraformens höjd. |
| [SetTopInShape](./settopinshape/) | Representerar den vertikala förskjutningen av formen från den översta kanten av föräldraformen, i enhet 1/4000 av föräldraformens höjd. |
| [GetLeftInShape](./getleftinshape/) | Representerar den horisontella förskjutningen av formen från den vänstra kanten av föräldraformen, i enhet 1/4000 av föräldraformens bredd. |
| [SetLeftInShape](./setleftinshape/) | Representerar den horisontella förskjutningen av formen från den vänstra kanten av föräldraformen, i enhet 1/4000 av föräldraformens bredd. |
| [GetWidthInShape](./getwidthinshape/) | Representerar bredden på formen, i enhet 1/4000 av föräldraformen. |
| [SetWidthInShape](./setwidthinshape/) | Representerar bredden på formen, i enhet 1/4000 av föräldraformen. |
| [GetHeightInShape](./getheightinshape/) | Representerar den vertikala förskjutningen av formen från den översta kanten av föräldraformen, i enhet 1/4000 av föräldraformens höjd. |
| [SetHeightInShape](./setheightinshape/) | Representerar den vertikala förskjutningen av formen från den översta kanten av föräldraformen, i enhet 1/4000 av föräldraformens höjd. |
| [GetGroup](./getgroup/) | Hämtar gruppformen som innehåller denna form. |
| [GetType](./gettype/) | Hämtar den automatiska formtypen. |
| [GetHasLine](./gethasline/) | Hämtar och anger om linjekanten på formen är synlig. |
| [SetHasLine](./sethasline/) | Hämtar och anger om linjekanten på formen är synlig. |
| [IsFilled](./isfilled/) | Indikerar om fyllningsformatet är synligt. |
| [SetIsFilled](./setisfilled/) | Indikerar om fyllningsformatet är synligt. |
| [IsFlippedHorizontally](./isflippedhorizontally/) | Hämtar och anger om formen är horisontellt speglad. |
| [SetIsFlippedHorizontally](./setisflippedhorizontally/) | Hämtar och anger om formen är horisontellt speglad. |
| [IsFlippedVertically](./isflippedvertically/) | Hämtar och anger om formen är vertikalt vänd . |
| [SetIsFlippedVertically](./setisflippedvertically/) | Hämtar och anger om formen är vertikalt vänd . |
| [GetActualLowerRightRow](./getactuallowerrightrow/) | Hämta den faktiska sista raden. |
| [GetConnectionPoints](./getconnectionpoints/) | Hämta anslutningspunkterna |
| [ToImage_ImageType](./toimage_imagetype/) | Skapar formens bild och sparar den till en ström i det angivna formatet. |
| [GetRelativeToOriginalPictureSize](./getrelativetooriginalpicturesize/) | Anger om formen är relativ till originalbildens storlek. |
| [SetRelativeToOriginalPictureSize](./setrelativetooriginalpicturesize/) | Anger om formen är relativ till originalbildens storlek. |
| [GetLinkedCell](./getlinkedcell/) | Hämtar eller anger arbetsbladsintervallet som är länkat till kontrollens värde. |
| [SetLinkedCell_String](./setlinkedcell_string/) | Hämtar eller anger arbetsbladsintervallet som är länkat till kontrollens värde. |
| [GetInputRange](./getinputrange/) | Hämtar eller anger arbetsbladsintervallet som används för att fylla den angivna kombinationsrutan. |
| [SetInputRange_String](./setinputrange_string/) | Hämtar eller anger arbetsbladsintervallet som används för att fylla den angivna kombinationsrutan. |
| [UpdateSelectedValue](./updateselectedvalue/) | Uppdatera det valda värdet med värdet från den länkade cellen. |
| [GetTextShapeType](./gettextshapetype/) | Hämtar och anger den förinställda textformstypen. |
| [SetTextShapeType](./settextshapetype/) | Hämtar och anger den förinställda textformstypen. |
| [GetTextBody](./gettextbody/) | Hämtar och anger inställningen för formens text. |
| [GetFont](./getfont/) | Representerar formens teckensnitt. |
| [SetFont](./setfont/) | Representerar formens teckensnitt. |
| [GetTextOptions](./gettextoptions/) | Representerar formens textalternativ. |
| [SetTextOptions](./settextoptions/) | Representerar formens textalternativ. |
| [CalculateTextSize](./calculatetextsize/) | Beräkna om textområdet |
| [GetText](./gettext/) | Hämtar och anger texten för denna form. |
| [SetText](./settext/) | Hämtar och anger texten för denna form. |
| [IsRichText](./isrichtext/) | Om texten är rik text. |
| [GetHtmlText](./gethtmltext/) | Hämtar och anger HTML-strängen som innehåller data och vissa format i den här textrutan. |
| [SetHtmlText](./sethtmltext/) | Hämtar och anger HTML-strängen som innehåller data och vissa format i den här textrutan. |
| [FormatCharacters](./formatcharacters/) | Formaterar vissa tecken med teckensnittsinställningen. |
| [Characters](./characters/) | Returnerar ett Characters-objekt som representerar ett teckenintervall inom texten. |
| [GetRichFormattings](./getrichformattings/) | Returnerar alla Characters-objekt som representerar ett teckenintervall inom texten . |
| [GetTextVerticalOverflow](./gettextverticaloverflow/) | Hämtar och anger den vertikala översvämningstypen för texten i formen som innehåller text. |
| [SetTextVerticalOverflow](./settextverticaloverflow/) | Hämtar och anger den vertikala översvämningstypen för texten i formen som innehåller text. |
| [GetTextHorizontalOverflow](./gettexthorizontaloverflow/) | Hämtar och anger den horisontella översvämningstypen för texten i formen som innehåller text. |
| [SetTextHorizontalOverflow](./settexthorizontaloverflow/) | Hämtar och anger den horisontella översvämningstypen för texten i formen som innehåller text. |
| [IsTextWrapped](./istextwrapped/) | Hämtar och anger den textbrytnings typen för formen som innehåller text. |
| [SetIsTextWrapped](./setistextwrapped/) | Hämtar och anger den textbrytnings typen för formen som innehåller text. |
| [GetTextOrientationType](./gettextorientationtype/) | Hämtar och anger textorienteringstypen för formen. |
| [SetTextOrientationType](./settextorientationtype/) | Hämtar och anger textorienteringstypen för formen. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Hämtar och anger den horisontella justeringstypen för texten i formen. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Hämtar och anger den horisontella justeringstypen för texten i formen. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Hämtar och anger den vertikala justeringstypen för texten i formen. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Hämtar och anger den vertikala justeringstypen för texten i formen. |
| [GetTextDirection](./gettextdirection/) | Hämtar/Sätter riktningen för textflödet för detta objekt. |
| [SetTextDirection](./settextdirection/) | Hämtar/Sätter riktningen för textflödet för detta objekt. |
| [GetTextBoxOptions](./gettextboxoptions/) | Hämtar textinformationen i formen |
| [GetControlData](./getcontroldata/) | Hämtar data för kontrollen. |
| [GetActiveXControl](./getactivexcontrol/) | Hämtar ActiveX-kontrollen. |
| [RemoveActiveXControl](./removeactivexcontrol/) | Ta bort activeX-kontrollen. |
| [GetPaths](./getpaths/) | Hämtar sökvägarna för en anpassad geometrisk form. |
| [GetGeometry](./getgeometry/) | Hämtar geometrin |
| [GetCreateId](./getcreateid/) | Hämtar och sätter skapa-id för denna form. |
| [SetCreateId](./setcreateid/) | Hämtar och sätter skapa-id för denna form. |
| [IsDecorative](./isdecorative/) | Anger om objektet är dekorativt. |
| [SetIsDecorative](./setisdecorative/) | Anger om objektet är dekorativt. |
| [GetActualBox](./getactualbox/) | Hämta den faktiska positionen och storleken på formen (efter att rotation, spegling osv. har tillämpats). |
| [FitToTextSize](./fittotextsize/) | Beräkna om ett textområde som är lämpligt för att visa allt textinnehåll. |
| [GetResultOfSmartArt](./getresultofsmartart/) | Konverterar smart art till grupperade former. |
| [IsSameSetting](./issamesetting/) | Returnerar om formen är densamma. |
