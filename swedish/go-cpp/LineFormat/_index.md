---
title: "LineFormat-klass"
linktitle: "LineFormat"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "LineFormat-klass. Inkapslar objektet som representerar linjeformat i Go."
type: docs
weight: 200
url: /sv/go-cpp/lineformat/
---

## LineFormat class

Representerar alla inställningar för linjen.

```go

type LineFormat struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewLineFormat](./newlineformat/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetHashCode](./gethashcode/) | Hämtar hashkoden. |
| [Equals](./equals/) | Bestämmer om detta objekt har samma värde som ett annat specificerat LineFormat-objekt. |
| [GetCompoundType](./getcompoundtype/) | Anger linjens sammansättningstyp. |
| [SetCompoundType](./setcompoundtype/) | Anger linjens sammansättningstyp. |
| [GetDashStyle](./getdashstyle/) | Anger linjens strecktyp. |
| [SetDashStyle](./setdashstyle/) | Anger linjens strecktyp. |
| [GetCapType](./getcaptype/) | Anger avslutningsändarna |
| [SetCapType](./setcaptype/) | Anger avslutningsändarna |
| [GetJoinType](./getjointype/) | Anger linjens sammanfogningstyp. |
| [SetJoinType](./setjointype/) | Anger linjens sammanfogningstyp. |
| [GetBeginArrowheadStyle](./getbeginarrowheadstyle/) | Hämtar och anger startpilens typ för linjen. |
| [SetBeginArrowheadStyle](./setbeginarrowheadstyle/) | Hämtar och anger startpilens typ för linjen. |
| [GetBeginArrowheadWidth](./getbeginarrowheadwidth/) | Hämtar och anger startpilens breddtyp för linjen. |
| [SetBeginArrowheadWidth](./setbeginarrowheadwidth/) | Hämtar och anger startpilens breddtyp för linjen. |
| [GetBeginArrowheadLength](./getbeginarrowheadlength/) | Hämtar och anger startpilens längdtyp för linjen. |
| [SetBeginArrowheadLength](./setbeginarrowheadlength/) | Hämtar och anger startpilens längdtyp för linjen. |
| [GetEndArrowheadStyle](./getendarrowheadstyle/) | Hämtar och anger slutpilens typ för linjen. |
| [SetEndArrowheadStyle](./setendarrowheadstyle/) | Hämtar och anger slutpilens typ för linjen. |
| [GetEndArrowheadWidth](./getendarrowheadwidth/) | Hämtar och anger slutpilens breddtyp för linjen. |
| [SetEndArrowheadWidth](./setendarrowheadwidth/) | Hämtar och anger slutpilens breddtyp för linjen. |
| [GetEndArrowheadLength](./getendarrowheadlength/) | Hämtar och anger slutpilens längdtyp för linjen. |
| [SetEndArrowheadLength](./setendarrowheadlength/) | Hämtar och anger slutpilens längdtyp för linjen. |
| [GetWeight](./getweight/) | Hämtar eller anger vikten på linjen i enheter av punkter. |
| [SetWeight](./setweight/) | Hämtar eller anger vikten på linjen i enheter av punkter. |
| [GetFillType](./getfilltype/) | Hämtar och anger fyllningstyp |
| [SetFillType](./setfilltype/) | Hämtar och anger fyllningstyp |
| [GetTransparency](./gettransparency/) | Returnerar eller anger graden av transparens för området som ett värde från 0.0 (opak) till 1.0 (klar). |
| [SetTransparency](./settransparency/) | Returnerar eller anger graden av transparens för området som ett värde från 0.0 (opak) till 1.0 (klar). |
| [GetGradientFill](./getgradientfill/) | Hämtar GradientFill-objektet. |
| [GetTextureFill](./gettexturefill/) | Hämtar TextureFill-objektet. |
| [GetSolidFill](./getsolidfill/) | Hämtar SolidFill-objektet. |
| [GetPatternFill](./getpatternfill/) | Hämtar PatternFill-objektet. |
| [GetGradientColorType](./getgradientcolortype/) | Returnerar gradientfärgstypen för den angivna fyllningen. |
| [GetGradientStyle](./getgradientstyle/) | Returnerar gradientstilen för den angivna fyllningen. |
| [GetGradientColor1](./getgradientcolor1/) | Returnerar gradientfärg 1 för den angivna fyllningen. |
| [GetGradientColor2](./getgradientcolor2/) | Returnerar gradientfärg 2 för den angivna fyllningen. |
| [GetGradientDegree](./getgradientdegree/) | Returnerar gradientgraden för den angivna fyllningen. Gäller endast för Excel 2007. |
| [GetGradientVariant](./getgradientvariant/) | Returnerar gradientvarianten för den angivna fyllningen. Gäller endast för Excel 2007. |
| [GetPresetColor](./getpresetcolor/) | Returnerar den förinställda gradientfärgen för den angivna fyllningen. |
| [SetOneColorGradient](./setonecolorgradient/) | Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast för Excel 2007. |
| [SetTwoColorGradient_Color_Color_GradientStyleType_Int](./settwocolorgradient_color_color_gradientstyletype_int/) | Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007. |
| [SetPresetColorGradient](./setpresetcolorgradient/) | Ställer in den angivna fyllningen till en förinställd färggradient. Gäller endast för Excel 2007. |
| [GetTexture](./gettexture/) | Representerar texturtypen för den angivna fyllningen. |
| [SetTexture](./settexture/) | Representerar texturtypen för den angivna fyllningen. |
| [GetPattern](./getpattern/) | Representerar ett områdes visningsmönster. |
| [SetPattern](./setpattern/) | Representerar ett områdes visningsmönster. |
| [GetPictureFormatType](./getpictureformattype/) | Hämtar och anger bildformattyp. |
| [SetPictureFormatType](./setpictureformattype/) | Hämtar och anger bildformattyp. |
| [GetScale](./getscale/) | Hämtar och anger skala för bildformat. |
| [SetScale](./setscale/) | Hämtar och anger skala för bildformat. |
| [GetImageData](./getimagedata/) | Hämtar och anger bilddata. |
| [SetImageData](./setimagedata/) | Hämtar och anger bilddata. |
