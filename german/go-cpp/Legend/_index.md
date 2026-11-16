---
title: "Legend Klasse"
linktitle: "Legend"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Legend-Klasse. Kapselt das Objekt, das legend in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/legend/
---

## Legend class

Kapselt das Objekt, das die Diagrammlegende darstellt.

```go

type Legend struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewLegend](./newlegend/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetPosition](./getposition/) | Liest oder legt den Legendenpositionstyp fest. |
| [SetPosition](./setposition/) | Liest oder legt den Legendenpositionstyp fest. |
| [GetLegendEntries](./getlegendentries/) | Liest eine Sammlung aller LegendEntry-Objekte in der angegebenen Diagrammlegende. Das Festlegen der Legenden­einträge des Oberflächendiagramms wird nicht unterstützt. Daher wird null zurückgegeben, wenn der Diagrammtyp ein Oberflächendiagramm ist. |
| [GetLegendLabels](./getlegendlabels/) | Liest die Beschriftungen der Legenden­einträge, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [IsOverLay](./isoverlay/) | Liest oder legt fest, ob die Legende angezeigt wird, ohne das Diagramm zu überlappen. |
| [SetIsOverLay](./setisoverlay/) | Liest oder legt fest, ob die Legende angezeigt wird, ohne das Diagramm zu überlappen. |
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
| [GetXRatioToChart](./getxratiotochart/) | Liest oder legt die X‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses zum Diagrammbereich fest. |
| [SetXRatioToChart](./setxratiotochart/) | Liest oder legt die X‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses zum Diagrammbereich fest. |
| [GetYRatioToChart](./getyratiotochart/) | Liest oder legt die Y‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses zum Diagrammbereich fest. |
| [SetYRatioToChart](./setyratiotochart/) | Liest oder legt die Y‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses zum Diagrammbereich fest. |
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
| [Characters](./characters/) | Gibt ein Characters-Objekt zurück, das einen Zeichenbereich innerhalb des Textes darstellt. |
| [GetReadingOrder](./getreadingorder/) | Stellt die Lesereihenfolge des Textes dar. |
| [SetReadingOrder](./setreadingorder/) | Stellt die Lesereihenfolge des Textes dar. |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | Liest oder legt fest, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. Auto-Anpassung bedeutet, dass der Text innerhalb einer Form skaliert wird, um den gesamten Text aufzunehmen. |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Liest oder legt fest, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. Auto-Anpassung bedeutet, dass der Text innerhalb einer Form skaliert wird, um den gesamten Text aufzunehmen. |
| [IsAutoText](./isautotext/) | Gibt an, dass der Text automatisch generiert wurde. |
| [SetIsAutoText](./setisautotext/) | Gibt an, dass der Text automatisch generiert wurde. |
| [GetText](./gettext/) | Liest oder legt den Text des Rahmentitels fest. |
| [SetText](./settext/) | Liest oder legt den Text des Rahmentitels fest. |
| [GetLinkedSource](./getlinkedsource/) | Liest und legt eine Referenz auf das Arbeitsblatt fest. |
| [SetLinkedSource](./setlinkedsource/) | Liest und legt eine Referenz auf das Arbeitsblatt fest. |
| [GetDirectionType](./getdirectiontype/) | Liest und legt die Schreibrichtung des Textes fest. |
| [SetDirectionType](./setdirectiontype/) | Liest und legt die Schreibrichtung des Textes fest. |
| [IsTextWrapped](./istextwrapped/) | Liest oder legt einen Wert fest, der angibt, ob der Text umgebrochen wird. |
| [SetIsTextWrapped](./setistextwrapped/) | Liest oder legt einen Wert fest, der angibt, ob der Text umgebrochen wird. |
