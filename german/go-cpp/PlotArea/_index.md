---
title: "PlotArea Klasse"
linktitle: "PlotArea"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PlotArea Klasse. Kapselt das Objekt, das den PlotArea in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/plotarea/
---

## PlotArea class

Kapselt das Objekt, das den Zeichenbereich in einem Diagramm darstellt.

```go

type PlotArea struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewPlotArea](./newplotarea/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetXRatioToChart](./getxratiotochart/) | Liest oder setzt die x‑Koordinate der oberen linken Ecke des Begrenzungsrahmens des Diagrammbereichs als Verhältnis zur Diagrammfläche. |
| [SetXRatioToChart](./setxratiotochart/) | Liest oder setzt die x‑Koordinate der oberen linken Ecke des Begrenzungsrahmens des Diagrammbereichs als Verhältnis zur Diagrammfläche. |
| [GetYRatioToChart](./getyratiotochart/) | Liest oder setzt die y‑Koordinate der oberen Ecke des Plot‑Bereichs‑Begrenzungsrahmens als Verhältnis zur Diagrammfläche. |
| [SetYRatioToChart](./setyratiotochart/) | Liest oder setzt die y‑Koordinate der oberen Ecke des Plot‑Bereichs‑Begrenzungsrahmens als Verhältnis zur Diagrammfläche. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Liest oder setzt die Höhe des Plot‑Bereichs‑Begrenzungsrahmens in Einheiten des Verhältnisses zur Diagrammfläche. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Liest oder setzt die Höhe des Plot‑Bereichs‑Begrenzungsrahmens in Einheiten des Verhältnisses zur Diagrammfläche. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Liest oder setzt die Breite des Plot‑Bereichs‑Begrenzungsrahmens in Einheiten des Verhältnisses zur Diagrammfläche. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Liest oder setzt die Breite des Plot‑Bereichs‑Begrenzungsrahmens in Einheiten des Verhältnisses zur Diagrammfläche. |
| [GetInnerXRatioToChart](./getinnerxratiotochart/) | Liest oder liest die x‑Koordinate der oberen Ecke des Plot‑Bereichs in Einheiten des Verhältnisses zur Diagrammfläche. |
| [SetInnerXRatioToChart](./setinnerxratiotochart/) | Liest oder liest die x‑Koordinate der oberen Ecke des Plot‑Bereichs in Einheiten des Verhältnisses zur Diagrammfläche. |
| [GetInnerYRatioToChart](./getinneryratiotochart/) | Liest oder liest die x‑Koordinate der oberen Ecke des Plot‑Bereichs in Einheiten des Verhältnisses zur Diagrammfläche. |
| [SetInnerYRatioToChart](./setinneryratiotochart/) | Liest oder liest die x‑Koordinate der oberen Ecke des Plot‑Bereichs in Einheiten des Verhältnisses zur Diagrammfläche. |
| [GetInnerHeightRatioToChart](./getinnerheightratiotochart/) | Liest oder setzt die Höhe des Plot‑Bereichs in Einheiten des Verhältnisses zur Diagrammfläche. |
| [SetInnerHeightRatioToChart](./setinnerheightratiotochart/) | Liest oder setzt die Höhe des Plot‑Bereichs in Einheiten des Verhältnisses zur Diagrammfläche. |
| [GetInnerWidthRatioToChart](./getinnerwidthratiotochart/) | Liest oder setzt die Breite des Plot‑Bereichs in Einheiten des Verhältnisses zur Diagrammfläche. |
| [SetInnerWidthRatioToChart](./setinnerwidthratiotochart/) | Liest oder setzt die Breite des Plot‑Bereichs in Einheiten des Verhältnisses zur Diagrammfläche. |
| [SetPositionAuto](./setpositionauto/) | Setzt die Position des Plot‑Bereichs auf automatisch. |
| [IsAutomaticSize](./isautomaticsize/) | Gibt an, ob der Plot‑Bereich automatisch dimensioniert wird. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Gibt an, ob der Plot‑Bereich automatisch dimensioniert wird. |
| [IsInnerMode](./isinnermode/) | Gibt an, ob die Größe des Plot‑Bereichs die Tick‑Markierungen und die Achsenbeschriftungen einschließt. False gibt an, dass die Größe die Größe des Plot‑Bereichs, der Tick‑Markierungen und der Achsenbeschriftungen bestimmen soll. |
| [SetIsInnerMode](./setisinnermode/) | Gibt an, ob die Größe des Plot‑Bereichs die Tick‑Markierungen und die Achsenbeschriftungen einschließt. False gibt an, dass die Größe die Größe des Plot‑Bereichs, der Tick‑Markierungen und der Achsenbeschriftungen bestimmen soll. |
| [GetShadow](./getshadow/) | True, wenn der Rahmen einen Schatten hat. |
| [SetShadow](./setshadow/) | True, wenn der Rahmen einen Schatten hat. |
| [GetShapeProperties](./getshapeproperties/) | Liest das ShapeProperties‑Objekt. |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | Gibt an, ob die Standardposition (DefaultX, DefaultY, DefaultWidth und DefaultHeight) festgelegt ist. |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Stellt das x der Standardposition in Einheiten des Bruchteils der Diagrammfläche dar. |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Stellt das y der Standardposition in Einheiten des Bruchteils der Diagrammfläche dar. |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Stellt die Breite der Standardposition in Einheiten des Bruchteils der Diagrammfläche dar. |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Stellt die Höhe der Standardposition in Einheiten des Bruchteils der Diagrammfläche dar. |
| [GetBorder](./getborder/) | Liest die Line</see>. |
| [GetArea](./getarea/) | Liest die Area</see>. |
| [GetTextOptions](./gettextoptions/) | Liest und setzt die Optionen des Textes. |
| [GetFont](./getfont/) | Liest ein Font‑Objekt des angegebenen ChartFrame‑Objekts. |
| [GetAutoScaleFont](./getautoscalefont/) | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße sich ändert. Der Standardwert ist True. |
| [SetAutoScaleFont](./setautoscalefont/) | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße sich ändert. Der Standardwert ist True. |
| [GetXPixel](./getxpixel/) | Liest oder setzt die x‑Koordinate der oberen linken Ecke in Pixeln. |
| [SetXPixel](./setxpixel/) | Liest oder setzt die x‑Koordinate der oberen linken Ecke in Pixeln. |
| [GetYPixel](./getypixel/) | Liest oder setzt die y‑Koordinate der oberen linken Ecke in Pixeln. |
| [SetYPixel](./setypixel/) | Liest oder setzt die y‑Koordinate der oberen linken Ecke in Pixeln. |
| [GetWidthPixel](./getwidthpixel/) | Liest oder setzt die Breite des Rahmens in Pixeln. |
| [SetWidthPixel](./setwidthpixel/) | Liest oder setzt die Breite des Rahmens in Pixeln. |
| [GetHeightPixel](./getheightpixel/) | Liest oder setzt die Höhe des Rahmens in Pixeln. |
| [SetHeightPixel](./setheightpixel/) | Liest oder setzt die Höhe des Rahmens in Pixeln. |
