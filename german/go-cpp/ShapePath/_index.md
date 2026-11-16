---
title: "ShapePath-Klasse"
linktitle: "ShapePath"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ShapePath-Klasse. Kapselt das Objekt, das shapepath in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/shapepath/
---

## ShapePath class

Stellt einen Erstellungsweg dar, der aus einer Reihe von Bewegungen, Linien und Kurven besteht, die zusammen eine geometrische Form bilden.

```go

type ShapePath struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewShapePath](./newshapepath/) | Initialisiert eine neue Instanz der ShapePath-Klasse. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetPathSegments](./getpathsegments/) | Ruft die ShapeSegmentPathCollection-Liste ab |
| [GetWidthPixel](./getwidthpixel/) | Ruft die Breite dieses Pfads in Pixeln ab. |
| [SetWidthPixel](./setwidthpixel/) | Ruft die Breite dieses Pfads in Pixeln ab. |
| [GetHeightPixel](./getheightpixel/) | Ruft die Höhe dieses Pfads in Pixeln ab. |
| [SetHeightPixel](./setheightpixel/) | Ruft die Höhe dieses Pfads in Pixeln ab. |
| [MoveTo](./moveto/) | Startet eine neue Figur vom angegebenen Punkt, ohne die aktuelle Figur zu schließen. Alle nachfolgenden Punkte, die dem Pfad hinzugefügt werden, werden zu dieser neuen Figur hinzugefügt. Einheit: Pixel. |
| [LineTo](./lineto/) | Fügt ein Liniensegment zur aktuellen Figur hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. Einheit: Pixel. |
| [CubicBezierTo](./cubicbezierto/) | Fügt der aktuellen Figur eine kubische Bézier-Kurve hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. Einheit: Pixel. |
| [ArcTo](./arcto/) | Fügt der aktuellen Figur einen elliptischen Bogen hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. |
| [Close](./close/) | Schließt die aktuelle Figur und startet eine neue Figur. Wenn die aktuelle Figur eine Sequenz verbundener Linien und Kurven enthält, schließt die Methode die Schleife, indem sie eine Linie vom Endpunkt zum Startpunkt verbindet. |
