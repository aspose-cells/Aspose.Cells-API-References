---
title: "LineFormat Klasse"
linktitle: "LineFormat"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "LineFormat Klasse. Kapselt das Objekt, das lineformat in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/lineformat/
---

## LineFormat class

Stellt alle Einstellungen der Linie dar.

```go

type LineFormat struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewLineFormat](./newlineformat/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetHashCode](./gethashcode/) | Ruft den Hashcode ab. |
| [Equals](./equals/) | Bestimmt, ob diese Instanz denselben Wert wie ein anderes angegebenes LineFormat-Objekt hat. |
| [GetCompoundType](./getcompoundtype/) | Gibt den Zeilenverbundtyp an. |
| [SetCompoundType](./setcompoundtype/) | Gibt den Zeilenverbundtyp an. |
| [GetDashStyle](./getdashstyle/) | Gibt den Strichtyp der Linie an. |
| [SetDashStyle](./setdashstyle/) | Gibt den Strichtyp der Linie an. |
| [GetCapType](./getcaptype/) | Gibt die Endkappen an. |
| [SetCapType](./setcaptype/) | Gibt die Endkappen an. |
| [GetJoinType](./getjointype/) | Gibt den Verbindungstyp der Linie an. |
| [SetJoinType](./setjointype/) | Gibt den Verbindungstyp der Linie an. |
| [GetBeginArrowheadStyle](./getbeginarrowheadstyle/) | Liest und setzt den Anfangspfeiltyp der Linie. |
| [SetBeginArrowheadStyle](./setbeginarrowheadstyle/) | Liest und setzt den Anfangspfeiltyp der Linie. |
| [GetBeginArrowheadWidth](./getbeginarrowheadwidth/) | Liest und setzt den Typ der Anfangspfeilbreite der Linie. |
| [SetBeginArrowheadWidth](./setbeginarrowheadwidth/) | Liest und setzt den Typ der Anfangspfeilbreite der Linie. |
| [GetBeginArrowheadLength](./getbeginarrowheadlength/) | Liest und setzt den Typ der Anfangspfeillänge der Linie. |
| [SetBeginArrowheadLength](./setbeginarrowheadlength/) | Liest und setzt den Typ der Anfangspfeillänge der Linie. |
| [GetEndArrowheadStyle](./getendarrowheadstyle/) | Liest und setzt den Typ des Endpfeils der Linie. |
| [SetEndArrowheadStyle](./setendarrowheadstyle/) | Liest und setzt den Typ des Endpfeils der Linie. |
| [GetEndArrowheadWidth](./getendarrowheadwidth/) | Liest und setzt den Typ der Endpfeilbreite der Linie. |
| [SetEndArrowheadWidth](./setendarrowheadwidth/) | Liest und setzt den Typ der Endpfeilbreite der Linie. |
| [GetEndArrowheadLength](./getendarrowheadlength/) | Liest und setzt den Typ der Endpfeillänge der Linie. |
| [SetEndArrowheadLength](./setendarrowheadlength/) | Liest und setzt den Typ der Endpfeillänge der Linie. |
| [GetWeight](./getweight/) | Liest oder setzt das Gewicht der Linie in Punkten. |
| [SetWeight](./setweight/) | Liest oder setzt das Gewicht der Linie in Punkten. |
| [GetFillType](./getfilltype/) | Liest und setzt den Fülltyp. |
| [SetFillType](./setfilltype/) | Liest und setzt den Fülltyp. |
| [GetTransparency](./gettransparency/) | Gibt den Transparenzgrad des Bereichs zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (klar). |
| [SetTransparency](./settransparency/) | Gibt den Transparenzgrad des Bereichs zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (klar). |
| [GetGradientFill](./getgradientfill/) | Liest das GradientFill-Objekt. |
| [GetTextureFill](./gettexturefill/) | Liest das TextureFill-Objekt. |
| [GetSolidFill](./getsolidfill/) | Liest das SolidFill-Objekt. |
| [GetPatternFill](./getpatternfill/) | Liest das PatternFill-Objekt. |
| [GetGradientColorType](./getgradientcolortype/) | Gibt den Farbtyp des Farbverlaufs für die angegebene Füllung zurück. |
| [GetGradientStyle](./getgradientstyle/) | Gibt den Stil des Farbverlaufs für die angegebene Füllung zurück. |
| [GetGradientColor1](./getgradientcolor1/) | Gibt die erste Farbverlauffarbe für die angegebene Füllung zurück. |
| [GetGradientColor2](./getgradientcolor2/) | Gibt die zweite Farbverlauffarbe für die angegebene Füllung zurück. |
| [GetGradientDegree](./getgradientdegree/) | Gibt den Grad des Farbverlaufs für die angegebene Füllung zurück. Gilt nur für Excel 2007. |
| [GetGradientVariant](./getgradientvariant/) | Gibt die Variante des Farbverlaufs für die angegebene Füllung zurück. Gilt nur für Excel 2007. |
| [GetPresetColor](./getpresetcolor/) | Gibt die voreingestellte Farbverlauffarbe für die angegebene Füllung zurück. |
| [SetOneColorGradient](./setonecolorgradient/) | Legt die angegebene Füllung auf einen einfarbigen Verlauf fest. Gilt nur für Excel 2007. |
| [SetTwoColorGradient_Color_Color_GradientStyleType_Int](./settwocolorgradient_color_color_gradientstyletype_int/) | Legt die angegebene Füllung auf einen zweifarbigen Verlauf fest. Gilt nur für Excel 2007. |
| [SetPresetColorGradient](./setpresetcolorgradient/) | Setzt die angegebene Füllung auf einen voreingestellten Farbverlauf. Gilt nur für Excel 2007. |
| [GetTexture](./gettexture/) | Stellt den Texturtyp für die angegebene Füllung dar. |
| [SetTexture](./settexture/) | Stellt den Texturtyp für die angegebene Füllung dar. |
| [GetPattern](./getpattern/) | Stellt das Anzeigemuster eines Bereichs dar. |
| [SetPattern](./setpattern/) | Stellt das Anzeigemuster eines Bereichs dar. |
| [GetPictureFormatType](./getpictureformattype/) | Liest und setzt den Bildformattyp. |
| [SetPictureFormatType](./setpictureformattype/) | Liest und setzt den Bildformattyp. |
| [GetScale](./getscale/) | Liest und setzt die Bildformatskala. |
| [SetScale](./setscale/) | Liest und setzt die Bildformatskala. |
| [GetImageData](./getimagedata/) | Liest und setzt die Bilddaten des Bildes. |
| [SetImageData](./setimagedata/) | Liest und setzt die Bilddaten des Bildes. |
