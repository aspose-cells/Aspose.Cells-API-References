---
title: "SparklineGroup Klasse"
linktitle: "SparklineGroup"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SparklineGroup Klasse. Kapselt das Objekt, das sparklinegroup in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/sparklinegroup/
---

## SparklineGroup class

<see cref=\"Sparkline\"/> ist in einer Sparkline-Gruppe organisiert. Eine SparklineGroup enthält eine variable Anzahl von Sparkline-Elementen. Eine Sparkline-Gruppe gibt den Typ, die Anzeigeeinstellungen und Achseneinstellungen für die Sparklines an.

```go

type SparklineGroup struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [ResetRanges](./resetranges/) | Setzt den Datenbereich und den Positionsbereich der Sparkline‑Gruppe zurück. Diese Methode löscht die ursprünglichen Sparkline‑Elemente in der Gruppe und erstellt neue Sparkline‑Elemente für die neuen Bereiche. |
| [GetPresetStyle](./getpresetstyle/) | Liest und setzt den voreingestellten Stiltyp der Sparkline‑Gruppe. |
| [SetPresetStyle](./setpresetstyle/) | Liest und setzt den voreingestellten Stiltyp der Sparkline‑Gruppe. |
| [GetSparklines](./getsparklines/) | Liest die Sammlung von Sparkline‑Objekten. |
| [GetType](./gettype/) | Gibt den Sparkline‑Typ der Sparkline‑Gruppe an. |
| [SetType](./settype/) | Gibt den Sparkline‑Typ der Sparkline‑Gruppe an. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Gibt an, wie leere Zellen dargestellt werden. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Gibt an, wie leere Zellen dargestellt werden. |
| [GetDisplayHidden](./getdisplayhidden/) | Gibt an, ob Daten in ausgeblendeten Zeilen und Spalten angezeigt werden sollen. |
| [SetDisplayHidden](./setdisplayhidden/) | Gibt an, ob Daten in ausgeblendeten Zeilen und Spalten angezeigt werden sollen. |
| [GetShowHighPoint](./getshowhighpoint/) | Gibt an, ob die höchsten Datenpunkte in der Sparkline-Gruppe hervorgehoben werden sollen. |
| [SetShowHighPoint](./setshowhighpoint/) | Gibt an, ob die höchsten Datenpunkte in der Sparkline-Gruppe hervorgehoben werden sollen. |
| [GetHighPointColor](./gethighpointcolor/) | Liest und setzt die Farbe der höchsten Datenpunkte in der Sparkline-Gruppe. |
| [SetHighPointColor](./sethighpointcolor/) | Liest und setzt die Farbe der höchsten Datenpunkte in der Sparkline-Gruppe. |
| [GetShowLowPoint](./getshowlowpoint/) | Gibt an, ob die niedrigsten Datenpunkte in der Sparkline-Gruppe hervorgehoben werden sollen. |
| [SetShowLowPoint](./setshowlowpoint/) | Gibt an, ob die niedrigsten Datenpunkte in der Sparkline-Gruppe hervorgehoben werden sollen. |
| [GetLowPointColor](./getlowpointcolor/) | Liest und setzt die Farbe der niedrigsten Datenpunkte in der Sparkline-Gruppe. |
| [SetLowPointColor](./setlowpointcolor/) | Liest und setzt die Farbe der niedrigsten Datenpunkte in der Sparkline-Gruppe. |
| [GetShowNegativePoints](./getshownegativepoints/) | Gibt an, ob negative Werte in der Sparkline-Gruppe mit einer anderen Farbe oder einem anderen Symbol hervorgehoben werden sollen. |
| [SetShowNegativePoints](./setshownegativepoints/) | Gibt an, ob negative Werte in der Sparkline-Gruppe mit einer anderen Farbe oder einem anderen Symbol hervorgehoben werden sollen. |
| [GetNegativePointsColor](./getnegativepointscolor/) | Liest und setzt die Farbe der negativen Werte in der Sparkline-Gruppe. |
| [SetNegativePointsColor](./setnegativepointscolor/) | Liest und setzt die Farbe der negativen Werte in der Sparkline-Gruppe. |
| [GetShowFirstPoint](./getshowfirstpoint/) | Gibt an, ob der erste Datenpunkt in der Sparkline-Gruppe hervorgehoben werden soll. |
| [SetShowFirstPoint](./setshowfirstpoint/) | Gibt an, ob der erste Datenpunkt in der Sparkline-Gruppe hervorgehoben werden soll. |
| [GetFirstPointColor](./getfirstpointcolor/) | Liest und setzt die Farbe des ersten Datenpunkts in der Sparkline-Gruppe. |
| [SetFirstPointColor](./setfirstpointcolor/) | Liest und setzt die Farbe des ersten Datenpunkts in der Sparkline-Gruppe. |
| [GetShowLastPoint](./getshowlastpoint/) | Gibt an, ob der letzte Datenpunkt in der Sparkline-Gruppe hervorgehoben werden soll. |
| [SetShowLastPoint](./setshowlastpoint/) | Gibt an, ob der letzte Datenpunkt in der Sparkline-Gruppe hervorgehoben werden soll. |
| [GetLastPointColor](./getlastpointcolor/) | Liest und setzt die Farbe des letzten Datenpunkts in der Sparkline-Gruppe. |
| [SetLastPointColor](./setlastpointcolor/) | Liest und setzt die Farbe des letzten Datenpunkts in der Sparkline-Gruppe. |
| [GetShowMarkers](./getshowmarkers/) | Gibt an, ob jeder Punkt in jeder Linien‑Sparkline in der Sparkline-Gruppe hervorgehoben werden soll. |
| [SetShowMarkers](./setshowmarkers/) | Gibt an, ob jeder Punkt in jeder Linien‑Sparkline in der Sparkline-Gruppe hervorgehoben werden soll. |
| [GetMarkersColor](./getmarkerscolor/) | Liest und setzt die Farbe der Punkte in jeder Linien‑Sparkline in der Sparkline-Gruppe. |
| [SetMarkersColor](./setmarkerscolor/) | Liest und setzt die Farbe der Punkte in jeder Linien‑Sparkline in der Sparkline-Gruppe. |
| [GetSeriesColor](./getseriescolor/) | Liest und setzt die Farbe der Sparklines in der Sparkline-Gruppe. |
| [SetSeriesColor](./setseriescolor/) | Liest und setzt die Farbe der Sparklines in der Sparkline-Gruppe. |
| [GetPlotRightToLeft](./getplotrighttoleft/) | Gibt an, ob die Plot‑Daten von rechts nach links verlaufen. |
| [SetPlotRightToLeft](./setplotrighttoleft/) | Gibt an, ob die Plot‑Daten von rechts nach links verlaufen. |
| [GetLineWeight](./getlineweight/) | Liest und setzt die Linienstärke in jeder Linien‑Sparkline in der Sparkline-Gruppe, in der Einheit Punkt. |
| [SetLineWeight](./setlineweight/) | Liest und setzt die Linienstärke in jeder Linien‑Sparkline in der Sparkline-Gruppe, in der Einheit Punkt. |
| [GetHorizontalAxisColor](./gethorizontalaxiscolor/) | Liest und setzt die Farbe der horizontalen Achse in der Sparkline-Gruppe. |
| [SetHorizontalAxisColor](./sethorizontalaxiscolor/) | Liest und setzt die Farbe der horizontalen Achse in der Sparkline-Gruppe. |
| [GetShowHorizontalAxis](./getshowhorizontalaxis/) | Gibt an, ob die horizontale Achse der Sparkline angezeigt wird. Die horizontale Achse erscheint, wenn die Sparkline Daten enthält, die die Nullachse überschreiten. |
| [SetShowHorizontalAxis](./setshowhorizontalaxis/) | Gibt an, ob die horizontale Achse der Sparkline angezeigt wird. Die horizontale Achse erscheint, wenn die Sparkline Daten enthält, die die Nullachse überschreiten. |
| [GetHorizontalAxisDateRange](./gethorizontalaxisdaterange/) | Stellt den Bereich dar, der die Datumswerte für die Sparkline-Daten enthält. |
| [SetHorizontalAxisDateRange](./sethorizontalaxisdaterange/) | Stellt den Bereich dar, der die Datumswerte für die Sparkline-Daten enthält. |
| [GetVerticalAxisMaxValueType](./getverticalaxismaxvaluetype/) | Stellt den Typ des maximalen Werts der vertikalen Achse dar. |
| [SetVerticalAxisMaxValueType](./setverticalaxismaxvaluetype/) | Stellt den Typ des maximalen Werts der vertikalen Achse dar. |
| [GetVerticalAxisMaxValue](./getverticalaxismaxvalue/) | Liest und setzt den benutzerdefinierten Maximalwert für die vertikale Achse. |
| [SetVerticalAxisMaxValue_Double](./setverticalaxismaxvalue_double/) | Liest und setzt den benutzerdefinierten Maximalwert für die vertikale Achse. |
| [SetVerticalAxisMaxValue_SparklineAxisMinMaxType_Double](./setverticalaxismaxvalue_sparklineaxisminmaxtype_double/) | Setzt den benutzerdefinierten Maximalwert für die vertikale Achse der Sparkline mit dem angegebenen Achsenwerttyp. |
| [SetVerticalAxisMinValue_SparklineAxisMinMaxType_Double](./setverticalaxisminvalue_sparklineaxisminmaxtype_double/) | Setzt den benutzerdefinierten Minimalwert für die vertikale Achse der Sparkline mit dem angegebenen Achsenwerttyp. |
| [GetVerticalAxisMinValueType](./getverticalaxisminvaluetype/) | Stellt den Typ des Minimalwerts der vertikalen Achse dar. |
| [SetVerticalAxisMinValueType](./setverticalaxisminvaluetype/) | Stellt den Typ des Minimalwerts der vertikalen Achse dar. |
| [GetVerticalAxisMinValue](./getverticalaxisminvalue/) | Liest und setzt den benutzerdefinierten Minimalwert für die vertikale Achse. |
| [SetVerticalAxisMinValue_Double](./setverticalaxisminvalue_double/) | Liest und setzt den benutzerdefinierten Minimalwert für die vertikale Achse. |
