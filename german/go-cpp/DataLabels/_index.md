---
title: "DataLabels Klasse"
linktitle: "DataLabels"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DataLabels Klasse. Kapselt das Objekt, das Datenbeschriftungen in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/datalabels/
---

## DataLabels class

Kapselt eine Sammlung aller DataLabel-Objekte für die angegebene Serie.

```go

type DataLabels struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewDataLabels](./newdatalabels/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetBorder](./getborder/) | Liest die Line</see>. |
| [GetArea](./getarea/) | Liest die Area</see>. |
| [IsAutoText](./isautotext/) | Gibt an, dass der Text automatisch generiert wurde. |
| [SetIsAutoText](./setisautotext/) | Gibt an, dass der Text automatisch generiert wurde. |
| [GetDirectionType](./getdirectiontype/) | Liest und legt die Schreibrichtung des Textes fest. |
| [SetDirectionType](./setdirectiontype/) | Liest und legt die Schreibrichtung des Textes fest. |
| [GetText](./gettext/) | Liest oder setzt den Text der Datenbeschriftung. |
| [SetText](./settext/) | Liest oder setzt den Text der Datenbeschriftung. |
| [IsTextWrapped](./istextwrapped/) | Liest oder legt einen Wert fest, der angibt, ob der Text umgebrochen wird. |
| [SetIsTextWrapped](./setistextwrapped/) | Liest oder legt einen Wert fest, der angibt, ob der Text umgebrochen wird. |
| [GetBackgroundMode](./getbackgroundmode/) | Liefert und setzt den Anzeigemodus des Hintergrunds |
| [SetBackgroundMode](./setbackgroundmode/) | Liefert und setzt den Anzeigemodus des Hintergrunds |
| [GetShowValue](./getshowvalue/) | Stellt das Anzeigeverhalten der Datenbeschriftungswerte eines angegebenen Diagramms dar. True zeigt die Werte an. False verbirgt sie. |
| [SetShowValue](./setshowvalue/) | Stellt das Anzeigeverhalten der Datenbeschriftungswerte eines angegebenen Diagramms dar. True zeigt die Werte an. False verbirgt sie. |
| [GetShowCellRange](./getshowcellrange/) | Gibt an, ob der Zellbereich als Datenbeschriftungen angezeigt werden soll. |
| [SetShowCellRange](./setshowcellrange/) | Gibt an, ob der Zellbereich als Datenbeschriftungen angezeigt werden soll. |
| [GetShowPercentage](./getshowpercentage/) | Stellt das Anzeigeverhalten des prozentualen Werts einer Datenbeschriftung eines angegebenen Diagramms dar. True zeigt den Prozentwert an. False verbirgt ihn. |
| [SetShowPercentage](./setshowpercentage/) | Stellt das Anzeigeverhalten des prozentualen Werts einer Datenbeschriftung eines angegebenen Diagramms dar. True zeigt den Prozentwert an. False verbirgt ihn. |
| [GetShowBubbleSize](./getshowbubblesize/) | Stellt das Anzeigeverhalten des prozentualen Werts einer Datenbeschriftung eines angegebenen Diagramms dar. True zeigt den Prozentwert an. False verbirgt den Prozentwert. |
| [SetShowBubbleSize](./setshowbubblesize/) | Stellt das Anzeigeverhalten des prozentualen Werts einer Datenbeschriftung eines angegebenen Diagramms dar. True zeigt den Prozentwert an. False verbirgt den Prozentwert. |
| [GetShowCategoryName](./getshowcategoryname/) | Stellt das Anzeigeverhalten des Kategorienamens einer Datenbeschriftung eines angegebenen Diagramms dar. True zeigt den Kategorienamen für die Datenbeschriftungen im Diagramm an. False verbirgt ihn. |
| [SetShowCategoryName](./setshowcategoryname/) | Stellt das Anzeigeverhalten des Kategorienamens einer Datenbeschriftung eines angegebenen Diagramms dar. True zeigt den Kategorienamen für die Datenbeschriftungen im Diagramm an. False verbirgt ihn. |
| [GetShowSeriesName](./getshowseriesname/) | Gibt an, ob der Serienname in den Datenbeschriftungen eines Diagramms angezeigt wird. True zeigt den Seriennamen an. False verbirgt ihn. |
| [SetShowSeriesName](./setshowseriesname/) | Gibt an, ob der Serienname in den Datenbeschriftungen eines Diagramms angezeigt wird. True zeigt den Seriennamen an. False verbirgt ihn. |
| [GetShowLegendKey](./getshowlegendkey/) | Stellt das Anzeigeverhalten des Legenden-Schlüssels einer Datenbeschriftung eines angegebenen Diagramms dar. True, wenn der Legenden-Schlüssel sichtbar ist. |
| [SetShowLegendKey](./setshowlegendkey/) | Stellt das Anzeigeverhalten des Legenden-Schlüssels einer Datenbeschriftung eines angegebenen Diagramms dar. True, wenn der Legenden-Schlüssel sichtbar ist. |
| [Get_NumberFormat](./get_numberformat/) | Stellt die Formatzeichenfolge für das DataLabels-Objekt dar. |
| [SetNumberFormat](./setnumberformat/) | Stellt die Formatzeichenfolge für das DataLabels-Objekt dar. |
| [GetNumber](./getnumber/) | Liest und setzt das integrierte Zahlenformat. |
| [SetNumber](./setnumber/) | Liest und setzt das integrierte Zahlenformat. |
| [GetNumberFormatLinked](./getnumberformatlinked/) | True, wenn das Zahlenformat mit den Zellen verknüpft ist (so dass sich das Zahlenformat in den Beschriftungen ändert, wenn es sich in den Zellen ändert). |
| [SetNumberFormatLinked](./setnumberformatlinked/) | True, wenn das Zahlenformat mit den Zellen verknüpft ist (so dass sich das Zahlenformat in den Beschriftungen ändert, wenn es sich in den Zellen ändert). |
| [ApplyFont](./applyfont/) | Wendet die Schriftart der Datenbeschriftungen auf alle untergeordneten Knoten an. |
| [GetFont](./getfont/) | Liest die Schriftart der DataLabels; |
| [GetSeparatorType](./getseparatortype/) | Liest oder setzt den Trennertyp, der für die Datenbeschriftungen in einem Diagramm verwendet wird. |
| [SetSeparatorType](./setseparatortype/) | Liest oder setzt den Trennertyp, der für die Datenbeschriftungen in einem Diagramm verwendet wird. |
| [GetSeparatorValue](./getseparatorvalue/) | Liest oder setzt den Trennwert, der für die Datenbeschriftungen in einem Diagramm verwendet wird. |
| [SetSeparatorValue](./setseparatorvalue/) | Liest oder setzt den Trennwert, der für die Datenbeschriftungen in einem Diagramm verwendet wird. |
| [GetPosition](./getposition/) | Stellt die Position der Datenbeschriftung dar. |
| [SetPosition](./setposition/) | Stellt die Position der Datenbeschriftung dar. |
| [IsNeverOverlap](./isneveroverlap/) | Gibt an, ob Datenbeschriftungen sich nie überlappen, wenn ein Kreisdiagramm in ein Bild umgewandelt wird. Hinweis: Diese Eigenschaft ist nur sinnvoll, wenn ein Kreisdiagramm in ein Bild umgewandelt wird. |
| [SetIsNeverOverlap](./setisneveroverlap/) | Gibt an, ob Datenbeschriftungen sich nie überlappen, wenn ein Kreisdiagramm in ein Bild umgewandelt wird. Hinweis: Diese Eigenschaft ist nur sinnvoll, wenn ein Kreisdiagramm in ein Bild umgewandelt wird. |
| [GetShapeType](./getshapetype/) | Liest oder setzt den Formtyp der Datenbeschriftung. |
| [SetShapeType](./setshapetype/) | Liest oder setzt den Formtyp der Datenbeschriftung. |
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
| [GetTextOptions](./gettextoptions/) | Liest und setzt die Optionen des Textes. |
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
| [GetLinkedSource](./getlinkedsource/) | Liest und legt eine Referenz auf das Arbeitsblatt fest. |
| [SetLinkedSource](./setlinkedsource/) | Liest und legt eine Referenz auf das Arbeitsblatt fest. |
