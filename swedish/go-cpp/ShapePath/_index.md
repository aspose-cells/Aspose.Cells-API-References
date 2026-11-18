---
title: "ShapePath klass"
linktitle: "ShapePath"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ShapePath klass. Innesluter objektet som representerar shapepath i Go."
type: docs
weight: 200
url: /sv/go-cpp/shapepath/
---

## ShapePath class

Representerar en skapandeväg bestående av en serie rörelser, linjer och kurvor som när de kombineras bildar en geometrisk form.

```go

type ShapePath struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewShapePath](./newshapepath/) | Initierar en ny instans av klassen ShapePath. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetPathSegments](./getpathsegments/) | Hämtar listan ShapeSegmentPathCollection |
| [GetWidthPixel](./getwidthpixel/) | Hämtar bredden på denna bana i enheten pixlar. |
| [SetWidthPixel](./setwidthpixel/) | Hämtar bredden på denna bana i enheten pixlar. |
| [GetHeightPixel](./getheightpixel/) | Hämtar höjden på denna bana i enheten pixlar. |
| [SetHeightPixel](./setheightpixel/) | Hämtar höjden på denna bana i enheten pixlar. |
| [MoveTo](./moveto/) | Startar en ny figur från den angivna punkten utan att stänga den aktuella figuren. Alla efterföljande punkter som läggs till i banan läggs till i denna nya figur. Enhet: Pixel. |
| [LineTo](./lineto/) | Lägger till ett linjesegment till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren. Enhet: Pixel. |
| [CubicBezierTo](./cubicbezierto/) | Lägger till en kubisk Bézier-kurva till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren. Enhet: Pixel. |
| [ArcTo](./arcto/) | Lägger till en elliptisk båge till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren. |
| [Close](./close/) | Stänger den aktuella figuren och startar en ny figur. Om den aktuella figuren innehåller en sekvens av sammanhängande linjer och kurvor, stänger metoden loopen genom att ansluta en linje från slutpunkten till startpunkten. |
