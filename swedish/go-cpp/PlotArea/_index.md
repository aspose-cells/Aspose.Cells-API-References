---
title: "PlotArea klass"
linktitle: "PlotArea"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PlotArea klass. Inkapslar objektet som representerar plotarea i Go."
type: docs
weight: 200
url: /sv/go-cpp/plotarea/
---

## PlotArea class

Inkapslar objektet som representerar plotområdet i ett diagram.

```go

type PlotArea struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewPlotArea](./newplotarea/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetXRatioToChart](./getxratiotochart/) | Hämtar eller anger x-koordinaten för den övre vänstra hörnet av plotområdets avgränsningsruta som en andel av diagramområdet. |
| [SetXRatioToChart](./setxratiotochart/) | Hämtar eller anger x-koordinaten för den övre vänstra hörnet av plotområdets avgränsningsruta som en andel av diagramområdet. |
| [GetYRatioToChart](./getyratiotochart/) | Hämtar eller anger y-koordinaten för den övre övre hörnet av plot-områdets avgränsningsruta som en andel av diagramområdet. |
| [SetYRatioToChart](./setyratiotochart/) | Hämtar eller anger y-koordinaten för den övre övre hörnet av plot-områdets avgränsningsruta som en andel av diagramområdet. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Hämtar eller anger höjden på plotområdets avgränsningsruta i enheter av förhållandet till diagramområdet. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Hämtar eller anger höjden på plotområdets avgränsningsruta i enheter av förhållandet till diagramområdet. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Hämtar eller anger bredden på plotområdets avgränsningsruta i enheter av förhållandet till diagramområdet. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Hämtar eller anger bredden på plotområdets avgränsningsruta i enheter av förhållandet till diagramområdet. |
| [GetInnerXRatioToChart](./getinnerxratiotochart/) | Hämtar eller hämtar x-koordinaten för det övre hörnet av plotområdet i enheter av förhållandet till diagramområdet. |
| [SetInnerXRatioToChart](./setinnerxratiotochart/) | Hämtar eller hämtar x-koordinaten för det övre hörnet av plotområdet i enheter av förhållandet till diagramområdet. |
| [GetInnerYRatioToChart](./getinneryratiotochart/) | Hämtar eller hämtar x-koordinaten för det övre hörnet av plotområdet i enheter av förhållandet till diagramområdet. |
| [SetInnerYRatioToChart](./setinneryratiotochart/) | Hämtar eller hämtar x-koordinaten för det övre hörnet av plotområdet i enheter av förhållandet till diagramområdet. |
| [GetInnerHeightRatioToChart](./getinnerheightratiotochart/) | Hämtar eller anger höjden på plotområdet i enheter av förhållandet till diagramområdet. |
| [SetInnerHeightRatioToChart](./setinnerheightratiotochart/) | Hämtar eller anger höjden på plotområdet i enheter av förhållandet till diagramområdet. |
| [GetInnerWidthRatioToChart](./getinnerwidthratiotochart/) | Hämtar eller anger bredden på plotområdet i enheter av förhållandet till diagramområdet. |
| [SetInnerWidthRatioToChart](./setinnerwidthratiotochart/) | Hämtar eller anger bredden på plotområdet i enheter av förhållandet till diagramområdet. |
| [SetPositionAuto](./setpositionauto/) | Ställ in positionen för plotområdet till automatisk |
| [IsAutomaticSize](./isautomaticsize/) | Indikerar om plotområdet är automatiskt storleksanpassat. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Indikerar om plotområdet är automatiskt storleksanpassat. |
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
| [GetXPixel](./getxpixel/) | Hämtar eller anger x-koordinaten för det övre vänstra hörnet i enheter av Pixel. |
| [SetXPixel](./setxpixel/) | Hämtar eller anger x-koordinaten för det övre vänstra hörnet i enheter av Pixel. |
| [GetYPixel](./getypixel/) | Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [SetYPixel](./setypixel/) | Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [GetWidthPixel](./getwidthpixel/) | Hämtar eller anger bredden på ramen i enheter av Pixel. |
| [SetWidthPixel](./setwidthpixel/) | Hämtar eller anger bredden på ramen i enheter av Pixel. |
| [GetHeightPixel](./getheightpixel/) | Hämtar eller anger höjden på ramen i enheter av pixlar. |
| [SetHeightPixel](./setheightpixel/) | Hämtar eller anger höjden på ramen i enheter av pixlar. |
