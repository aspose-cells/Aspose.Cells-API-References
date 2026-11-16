---
title: "Title Klasse"
linktitle: "Title"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Title Klasse. Kapselt das Objekt, das den Titel in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/title/
---

## Title class

Kapselt das Objekt, das den Titel eines Diagramms oder einer Achse darstellt.

```go

type Title struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewTitle](./newtitle/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetText](./gettext/) | Liest oder setzt den Text der Anzeigeeinheitenbeschriftung. |
| [SetText](./settext/) | Liest oder setzt den Text der Anzeigeeinheitenbeschriftung. |
| [IsVisible](./isvisible/) | Stellt dar, ob der Titel sichtbar ist. |
| [SetIsVisible](./setisvisible/) | Stellt dar, ob der Titel sichtbar ist. |
| [GetXRatioToChart](./getxratiotochart/) | Liest oder setzt die x-Koordinate der oberen linken Ecke in Einheiten des Bruchteils des Diagrammbereichs. X in Pixeln = XRatioToChart * Chart.ChartObject.Width; |
| [SetXRatioToChart](./setxratiotochart/) | Liest oder setzt die x-Koordinate der oberen linken Ecke in Einheiten des Bruchteils des Diagrammbereichs. X in Pixeln = XRatioToChart * Chart.ChartObject.Width; |
| [GetYRatioToChart](./getyratiotochart/) | Liest oder setzt die y-Koordinate der oberen linken Ecke in Einheiten des Bruchteils des Diagrammbereichs. Y in Pixeln = YRatioToChart * Chart.ChartObject.Width; |
| [SetYRatioToChart](./setyratiotochart/) | Liest oder setzt die y-Koordinate der oberen linken Ecke in Einheiten des Bruchteils des Diagrammbereichs. Y in Pixeln = YRatioToChart * Chart.ChartObject.Width; |
| [GetOverLay](./getoverlay/) | Stellt einen überlagerten, zentrierten Titel in einem Diagramm dar, ohne das Diagramm zu skalieren. |
| [SetOverLay](./setoverlay/) | Stellt einen überlagerten, zentrierten Titel in einem Diagramm dar, ohne das Diagramm zu skalieren. |
| [Characters](./characters/) | Liest die Rich-Text-Formatierung dieses Titels. |
| [Characters_Int_Int](./characters_int_int/) | Gibt ein Characters-Objekt zurück, das einen Zeichenbereich innerhalb des Textes darstellt. |
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
| [IsAutomaticSize](./isautomaticsize/) | Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Gibt an, ob der Diagrammrahmen automatisch dimensioniert ist. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Liest oder legt die Breite des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich fest. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Liest oder legt die Breite des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich fest. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Liest oder legt die Höhe des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich fest. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Liest oder legt die Höhe des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich fest. |
| [GetXPixel](./getxpixel/) | Liest oder setzt die x‑Koordinate der oberen linken Ecke in Pixeln. |
| [SetXPixel](./setxpixel/) | Liest oder setzt die x‑Koordinate der oberen linken Ecke in Pixeln. |
| [GetYPixel](./getypixel/) | Liest oder setzt die y‑Koordinate der oberen linken Ecke in Pixeln. |
| [SetYPixel](./setypixel/) | Liest oder setzt die y‑Koordinate der oberen linken Ecke in Pixeln. |
| [GetWidthPixel](./getwidthpixel/) | Liest oder setzt die Breite des Rahmens in Pixeln. |
| [SetWidthPixel](./setwidthpixel/) | Liest oder setzt die Breite des Rahmens in Pixeln. |
| [GetHeightPixel](./getheightpixel/) | Liest oder setzt die Höhe des Rahmens in Pixeln. |
| [SetHeightPixel](./setheightpixel/) | Liest oder setzt die Höhe des Rahmens in Pixeln. |
| [SetPositionAuto](./setpositionauto/) | Setze die Position des Rahmens auf automatisch |
| [IsDeleted](./isdeleted/) | Gibt an, ob diese Datenbeschriftung gelöscht wurde. |
| [SetIsDeleted](./setisdeleted/) | Gibt an, ob diese Datenbeschriftung gelöscht wurde. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Liest und legt die horizontale Ausrichtung des Textes fest. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Liest und legt die horizontale Ausrichtung des Textes fest. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Liest oder legt die vertikale Ausrichtung des Textes fest. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Liest oder legt die vertikale Ausrichtung des Textes fest. |
| [GetRotationAngle](./getrotationangle/) | Stellt den Drehwinkel des Textes dar. |
| [SetRotationAngle](./setrotationangle/) | Stellt den Drehwinkel des Textes dar. |
| [IsAutomaticRotation](./isautomaticrotation/) | Gibt an, ob der Text des Diagramms automatisch gedreht wird. |
| [GetReadingOrder](./getreadingorder/) | Stellt die Lesereihenfolge des Textes dar. |
| [SetReadingOrder](./setreadingorder/) | Stellt die Lesereihenfolge des Textes dar. |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | Liest oder legt fest, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. Auto-Anpassung bedeutet, dass der Text innerhalb einer Form skaliert wird, um den gesamten Text aufzunehmen. |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Liest oder legt fest, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. Auto-Anpassung bedeutet, dass der Text innerhalb einer Form skaliert wird, um den gesamten Text aufzunehmen. |
| [IsAutoText](./isautotext/) | Gibt an, dass der Text automatisch generiert wurde. |
| [SetIsAutoText](./setisautotext/) | Gibt an, dass der Text automatisch generiert wurde. |
| [GetLinkedSource](./getlinkedsource/) | Liest und legt eine Referenz auf das Arbeitsblatt fest. |
| [SetLinkedSource](./setlinkedsource/) | Liest und legt eine Referenz auf das Arbeitsblatt fest. |
| [GetDirectionType](./getdirectiontype/) | Liest und legt die Schreibrichtung des Textes fest. |
| [SetDirectionType](./setdirectiontype/) | Liest und legt die Schreibrichtung des Textes fest. |
| [IsTextWrapped](./istextwrapped/) | Liest oder legt einen Wert fest, der angibt, ob der Text umgebrochen wird. |
| [SetIsTextWrapped](./setistextwrapped/) | Liest oder legt einen Wert fest, der angibt, ob der Text umgebrochen wird. |
