---
title: "DataLabels‑klass"
linktitle: "DataLabels"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DataLabels‑klass. Inkapslar objektet som representerar datalabels i Go."
type: docs
weight: 200
url: /sv/go-cpp/datalabels/
---

## DataLabels class

Inkapslar en samling av alla DataLabel-objekt för den angivna Series.

```go

type DataLabels struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewDataLabels](./newdatalabels/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetBorder](./getborder/) | Hämtar Line</see>. |
| [GetArea](./getarea/) | Hämtar Area</see>. |
| [IsAutoText](./isautotext/) | Anger att texten är automatiskt genererad. |
| [SetIsAutoText](./setisautotext/) | Anger att texten är automatiskt genererad. |
| [GetDirectionType](./getdirectiontype/) | Hämtar eller anger textens riktning. |
| [SetDirectionType](./setdirectiontype/) | Hämtar eller anger textens riktning. |
| [GetText](./gettext/) | Hämtar eller anger texten för datamärket. |
| [SetText](./settext/) | Hämtar eller anger texten för datamärket. |
| [IsTextWrapped](./istextwrapped/) | Hämtar eller anger ett värde som indikerar om texten är radbruten. |
| [SetIsTextWrapped](./setistextwrapped/) | Hämtar eller anger ett värde som indikerar om texten är radbruten. |
| [GetBackgroundMode](./getbackgroundmode/) | Hämtar och anger visningsläget för bakgrunden |
| [SetBackgroundMode](./setbackgroundmode/) | Hämtar och anger visningsläget för bakgrunden |
| [GetShowValue](./getshowvalue/) | Representerar ett specificerat diagrammets datamärkesvärdens visningsbeteende. True visar värdena. False döljer dem. |
| [SetShowValue](./setshowvalue/) | Representerar ett specificerat diagrammets datamärkesvärdens visningsbeteende. True visar värdena. False döljer dem. |
| [GetShowCellRange](./getshowcellrange/) | Anger om cellintervallet ska visas som datamärken. |
| [SetShowCellRange](./setshowcellrange/) | Anger om cellintervallet ska visas som datamärken. |
| [GetShowPercentage](./getshowpercentage/) | Representerar ett specificerat diagrammets dataetiketts procentvärdes visningsbeteende. True visar procentvärdet. False för att dölja. |
| [SetShowPercentage](./setshowpercentage/) | Representerar ett specificerat diagrammets dataetiketts procentvärdes visningsbeteende. True visar procentvärdet. False för att dölja. |
| [GetShowBubbleSize](./getshowbubblesize/) | Representerar ett specificerat diagrammets dataetiketts procentvärdes visningsbeteende.True visar procentvärdet.False döljer procentvärdet. |
| [SetShowBubbleSize](./setshowbubblesize/) | Representerar ett specificerat diagrammets dataetiketts procentvärdes visningsbeteende.True visar procentvärdet.False döljer procentvärdet. |
| [GetShowCategoryName](./getshowcategoryname/) | Representerar ett specificerat diagrammets dataetiketts kategorinamnvisningsbeteende.True för att visa kategorinamnet för dataetiketterna på ett diagram. False för att dölja. |
| [SetShowCategoryName](./setshowcategoryname/) | Representerar ett specificerat diagrammets dataetiketts kategorinamnvisningsbeteende.True för att visa kategorinamnet för dataetiketterna på ett diagram. False för att dölja. |
| [GetShowSeriesName](./getshowseriesname/) | Indikerar om serienamnet visas på dataetiketterna i ett diagram.True för att visa serienamnet.False för att dölja. |
| [SetShowSeriesName](./setshowseriesname/) | Indikerar om serienamnet visas på dataetiketterna i ett diagram.True för att visa serienamnet.False för att dölja. |
| [GetShowLegendKey](./getshowlegendkey/) | Representerar ett specificerat diagrammets dataetiketts legendnyckels visningsbeteende.True om legendnyckeln för dataetiketten är synlig. |
| [SetShowLegendKey](./setshowlegendkey/) | Representerar ett specificerat diagrammets dataetiketts legendnyckels visningsbeteende.True om legendnyckeln för dataetiketten är synlig. |
| [Get_NumberFormat](./get_numberformat/) | Representerar formatsträngen för DataLabels-objektet. |
| [SetNumberFormat](./setnumberformat/) | Representerar formatsträngen för DataLabels-objektet. |
| [GetNumber](./getnumber/) | Hämtar och anger det inbyggda talformatet. |
| [SetNumber](./setnumber/) | Hämtar och anger det inbyggda talformatet. |
| [GetNumberFormatLinked](./getnumberformatlinked/) | Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna). |
| [SetNumberFormatLinked](./setnumberformatlinked/) | Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna). |
| [ApplyFont](./applyfont/) | Applicera teckensnittet för dataetiketterna på alla underordnade noder. |
| [GetFont](./getfont/) | Hämtar teckensnittet för DataLabels; |
| [GetSeparatorType](./getseparatortype/) | Hämtar eller anger separator‑typen som används för dataetiketterna i ett diagram. |
| [SetSeparatorType](./setseparatortype/) | Hämtar eller anger separator‑typen som används för dataetiketterna i ett diagram. |
| [GetSeparatorValue](./getseparatorvalue/) | Hämtar eller anger separator‑värdet som används för dataetiketterna i ett diagram. |
| [SetSeparatorValue](./setseparatorvalue/) | Hämtar eller anger separator‑värdet som används för dataetiketterna i ett diagram. |
| [GetPosition](./getposition/) | Representerar positionen för dataetiketten. |
| [SetPosition](./setposition/) | Representerar positionen för dataetiketten. |
| [IsNeverOverlap](./isneveroverlap/) | Indikerar om Datalabels aldrig överlappar när en Pie Chart konverteras till bild.Obs: den här egenskapen är endast meningsfull när en Pie Chart konverteras till bild. |
| [SetIsNeverOverlap](./setisneveroverlap/) | Indikerar om Datalabels aldrig överlappar när en Pie Chart konverteras till bild.Obs: den här egenskapen är endast meningsfull när en Pie Chart konverteras till bild. |
| [GetShapeType](./getshapetype/) | Hämtar eller anger  formtypen för dataetiketten. |
| [SetShapeType](./setshapetype/) | Hämtar eller anger  formtypen för dataetiketten. |
| [IsInnerMode](./isinnermode/) | Indikerar om storleken på plotområdet inkluderar tick-markeringar och axelrubriker. False anger att storleken ska bestämma storleken på plotområdet, tick-markeringarna och axelrubrikerna. |
| [SetIsInnerMode](./setisinnermode/) | Indikerar om storleken på plotområdet inkluderar tick-markeringar och axelrubriker. False anger att storleken ska bestämma storleken på plotområdet, tick-markeringarna och axelrubrikerna. |
| [GetShadow](./getshadow/) | Sant om ramen har en skugga. |
| [SetShadow](./setshadow/) | Sant om ramen har en skugga. |
| [GetShapeProperties](./getshapeproperties/) | Hämtar ShapeProperties-objektet. |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | Indikerar om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är angiven. |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Representerar x för standardpositionen i enheter av bråkdel av diagramområdet. |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Representerar y för standardpositionen i enheter av bråkdel av diagramområdet. |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Representerar bredden för standardpositionen i enheter av bråkdel av diagramområdet. |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Representerar höjden för standardpositionen i enheter av bråkdel av diagramområdet. |
| [GetTextOptions](./gettextoptions/) | Hämtar och anger alternativen för texten. |
| [GetAutoScaleFont](./getautoscalefont/) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant. |
| [SetAutoScaleFont](./setautoscalefont/) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant. |
| [IsAutomaticSize](./isautomaticsize/) | Anger om diagramramen har automatisk storlek. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Anger om diagramramen har automatisk storlek. |
| [GetXRatioToChart](./getxratiotochart/) | Hämtar eller anger x-koordinaten för det övre vänstra hörnet i enheter av förhållandet till diagramområdet. |
| [SetXRatioToChart](./setxratiotochart/) | Hämtar eller anger x-koordinaten för det övre vänstra hörnet i enheter av förhållandet till diagramområdet. |
| [GetYRatioToChart](./getyratiotochart/) | Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av förhållandet till diagramområdet. |
| [SetYRatioToChart](./setyratiotochart/) | Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av förhållandet till diagramområdet. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Hämtar eller anger ramens bredd i enheter av förhållandet till diagramområdet. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Hämtar eller anger ramens bredd i enheter av förhållandet till diagramområdet. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Hämtar eller anger ramens höjd i enheter av förhållandet till diagramområdet. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Hämtar eller anger ramens höjd i enheter av förhållandet till diagramområdet. |
| [GetXPixel](./getxpixel/) | Hämtar eller anger x-koordinaten för det övre vänstra hörnet i enheter av Pixel. |
| [SetXPixel](./setxpixel/) | Hämtar eller anger x-koordinaten för det övre vänstra hörnet i enheter av Pixel. |
| [GetYPixel](./getypixel/) | Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [SetYPixel](./setypixel/) | Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [GetWidthPixel](./getwidthpixel/) | Hämtar eller anger bredden på ramen i enheter av Pixel. |
| [SetWidthPixel](./setwidthpixel/) | Hämtar eller anger bredden på ramen i enheter av Pixel. |
| [GetHeightPixel](./getheightpixel/) | Hämtar eller anger höjden på ramen i enheter av pixlar. |
| [SetHeightPixel](./setheightpixel/) | Hämtar eller anger höjden på ramen i enheter av pixlar. |
| [SetPositionAuto](./setpositionauto/) | Ställ in ramens position till automatisk |
| [IsDeleted](./isdeleted/) | Anger om denna datamärkning är raderad. |
| [SetIsDeleted](./setisdeleted/) | Anger om denna datamärkning är raderad. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Hämtar och anger textens horisontella justering. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Hämtar och anger textens horisontella justering. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Hämtar eller anger textens vertikala justering. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Hämtar eller anger textens vertikala justering. |
| [GetRotationAngle](./getrotationangle/) | Representerar textens rotationsvinkel. |
| [SetRotationAngle](./setrotationangle/) | Representerar textens rotationsvinkel. |
| [IsAutomaticRotation](./isautomaticrotation/) | Anger om diagramtexten roteras automatiskt. |
| [Characters](./characters/) | Returnerar ett Characters-objekt som representerar ett teckenintervall inom texten. |
| [GetReadingOrder](./getreadingorder/) | Representerar läsordning för text. |
| [SetReadingOrder](./setreadingorder/) | Representerar läsordning för text. |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | Hämtar eller anger om en form ska anpassas automatiskt för att helt innehålla den text som beskrivs i den. Automatisk anpassning innebär att texten inom en form skalas för att rymma all text. |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Hämtar eller anger om en form ska anpassas automatiskt för att helt innehålla den text som beskrivs i den. Automatisk anpassning innebär att texten inom en form skalas för att rymma all text. |
| [GetLinkedSource](./getlinkedsource/) | Hämtar och anger en referens till arbetsbladet. |
| [SetLinkedSource](./setlinkedsource/) | Hämtar och anger en referens till arbetsbladet. |
