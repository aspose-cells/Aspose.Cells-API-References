---
title: "ChartTextFrame-klass"
linktitle: "ChartTextFrame"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ChartTextFrame-klass. Inkapslar objektet som representerar charttextframe i Go."
type: docs
weight: 200
url: /sv/go-cpp/charttextframe/
---

## ChartTextFrame class

Inkapslar objektet som representerar ramobjektet som innehåller text.

```go

type ChartTextFrame struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewChartTextFrame](./newcharttextframe/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
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
| [IsAutoText](./isautotext/) | Anger att texten är automatiskt genererad. |
| [SetIsAutoText](./setisautotext/) | Anger att texten är automatiskt genererad. |
| [GetText](./gettext/) | Hämtar eller anger texten för en ramtitel. |
| [SetText](./settext/) | Hämtar eller anger texten för en ramtitel. |
| [GetLinkedSource](./getlinkedsource/) | Hämtar och anger en referens till arbetsbladet. |
| [SetLinkedSource](./setlinkedsource/) | Hämtar och anger en referens till arbetsbladet. |
| [GetDirectionType](./getdirectiontype/) | Hämtar eller anger textens riktning. |
| [SetDirectionType](./setdirectiontype/) | Hämtar eller anger textens riktning. |
| [IsTextWrapped](./istextwrapped/) | Hämtar eller anger ett värde som indikerar om texten är radbruten. |
| [SetIsTextWrapped](./setistextwrapped/) | Hämtar eller anger ett värde som indikerar om texten är radbruten. |
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
| [GetBorder](./getborder/) | Hämtar Line</see>. |
| [GetArea](./getarea/) | Hämtar Area</see>. |
| [GetTextOptions](./gettextoptions/) | Hämtar och anger alternativen för texten. |
| [GetFont](./getfont/) | Hämtar ett Font-objekt för det angivna ChartFrame-objektet. |
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
