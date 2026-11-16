---
title: "Achsenklasse"
linktitle: "Achse"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Achsenklasse. Kapselt das Objekt, das die Achse in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/axis/
---

## Axis class

Kapselt das Objekt, das eine Achse eines Diagramms darstellt.

```go

type Axis struct  {
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
| [GetArea](./getarea/) | Ermittelt die Fläche. |
| [IsAutomaticMinValue](./isautomaticminvalue/) | Gibt an, ob der Minimalwert automatisch zugewiesen wird. |
| [SetIsAutomaticMinValue](./setisautomaticminvalue/) | Gibt an, ob der Minimalwert automatisch zugewiesen wird. |
| [GetMinValue](./getminvalue/) | Stellt den Minimalwert auf der Werteachse dar. |
| [SetMinValue](./setminvalue/) | Stellt den Minimalwert auf der Werteachse dar. |
| [IsAutomaticMaxValue](./isautomaticmaxvalue/) | Gibt an, ob der Maximalwert automatisch zugewiesen wird. |
| [SetIsAutomaticMaxValue](./setisautomaticmaxvalue/) | Gibt an, ob der Maximalwert automatisch zugewiesen wird. |
| [GetMaxValue](./getmaxvalue/) | Stellt den Maximalwert auf der Werteachse dar. |
| [SetMaxValue](./setmaxvalue/) | Stellt den Maximalwert auf der Werteachse dar. |
| [IsAutomaticMajorUnit](./isautomaticmajorunit/) | Gibt an, ob die Haupteinheit der Achse automatisch zugewiesen wird. |
| [SetIsAutomaticMajorUnit](./setisautomaticmajorunit/) | Gibt an, ob die Haupteinheit der Achse automatisch zugewiesen wird. |
| [GetMajorUnit](./getmajorunit/) | Stellt die Haupteinheiten für die Achse dar. |
| [SetMajorUnit](./setmajorunit/) | Stellt die Haupteinheiten für die Achse dar. |
| [IsAutomaticMinorUnit](./isautomaticminorunit/) | Gibt an, ob die Nebeneinheit der Achse automatisch zugewiesen wird. |
| [SetIsAutomaticMinorUnit](./setisautomaticminorunit/) | Gibt an, ob die Nebeneinheit der Achse automatisch zugewiesen wird. |
| [GetMinorUnit](./getminorunit/) | Stellt die Nebeneinheiten für die Achse dar. |
| [SetMinorUnit](./setminorunit/) | Stellt die Nebeneinheiten für die Achse dar. |
| [GetAxisLine](./getaxisline/) | Ermittelt das Aussehen einer Achse. |
| [GetMajorTickMark](./getmajortickmark/) | Stellt den Typ des Hauptteilstrichs für die angegebene Achse dar. |
| [SetMajorTickMark](./setmajortickmark/) | Stellt den Typ des Hauptteilstrichs für die angegebene Achse dar. |
| [GetMinorTickMark](./getminortickmark/) | Stellt den Typ des Nebenteilstrichs für die angegebene Achse dar. |
| [SetMinorTickMark](./setminortickmark/) | Stellt den Typ des Nebenteilstrichs für die angegebene Achse dar. |
| [GetTickLabelPosition](./getticklabelposition/) | Stellt die Position der Teilstrichbeschriftungen auf der angegebenen Achse dar. |
| [SetTickLabelPosition](./setticklabelposition/) | Stellt die Position der Teilstrichbeschriftungen auf der angegebenen Achse dar. |
| [GetCrossAt](./getcrossat/) | Stellt den Punkt auf der Werteachse dar, an dem die Kategorienachse sie schneidet. |
| [SetCrossAt](./setcrossat/) | Stellt den Punkt auf der Werteachse dar, an dem die Kategorienachse sie schneidet. |
| [GetCrossType](./getcrosstype/) | Stellt den Kreuzungstyp auf der angegebenen Achse dar, an dem die andere Achse kreuzt. |
| [SetCrossType](./setcrosstype/) | Stellt den Kreuzungstyp auf der angegebenen Achse dar, an dem die andere Achse kreuzt. |
| [GetLogBase](./getlogbase/) | Stellt die logarithmische Basis dar. Der Standardwert ist 10. |
| [SetLogBase](./setlogbase/) | Stellt die logarithmische Basis dar. Der Standardwert ist 10. |
| [IsLogarithmic](./islogarithmic/) | Stellt dar, ob der Skalierungstyp der Werteachse logarithmisch ist oder nicht. |
| [SetIsLogarithmic](./setislogarithmic/) | Stellt dar, ob der Skalierungstyp der Werteachse logarithmisch ist oder nicht. |
| [IsPlotOrderReversed](./isplotorderreversed/) | Stellt dar, ob Microsoft Excel Datenpunkte von zuletzt nach zuerst plottet. |
| [SetIsPlotOrderReversed](./setisplotorderreversed/) | Stellt dar, ob Microsoft Excel Datenpunkte von zuletzt nach zuerst plottet. |
| [GetAxisBetweenCategories](./getaxisbetweencategories/) | Stellt dar, ob die Werteachse die Kategorienachse zwischen den Kategorien schneidet. |
| [SetAxisBetweenCategories](./setaxisbetweencategories/) | Stellt dar, ob die Werteachse die Kategorienachse zwischen den Kategorien schneidet. |
| [GetTickLabels](./getticklabels/) | Gibt ein TickLabels-Objekt zurück, das die Teilstrichbeschriftungen für die angegebene Achse darstellt. |
| [GetTickLabelSpacing](./getticklabelspacing/) | Stellt die Anzahl der Kategorien oder Reihen zwischen Teilstrichbeschriftungen dar. Gilt nur für Kategorien- und Reihenachsen. |
| [SetTickLabelSpacing](./setticklabelspacing/) | Stellt die Anzahl der Kategorien oder Reihen zwischen Teilstrichbeschriftungen dar. Gilt nur für Kategorien- und Reihenachsen. |
| [IsAutoTickLabelSpacing](./isautoticklabelspacing/) | Gibt an, ob der Abstand der Teilstrichbeschriftung automatisch ist |
| [SetIsAutoTickLabelSpacing](./setisautoticklabelspacing/) | Gibt an, ob der Abstand der Teilstrichbeschriftung automatisch ist |
| [GetTickMarkSpacing](./gettickmarkspacing/) | Gibt die Anzahl der Kategorien oder Reihen zwischen Teilstrichen zurück oder legt sie fest. Gilt nur für Kategorien- und Reihenachsen. |
| [SetTickMarkSpacing](./settickmarkspacing/) | Gibt die Anzahl der Kategorien oder Reihen zwischen Teilstrichen zurück oder legt sie fest. Gilt nur für Kategorien- und Reihenachsen. |
| [GetDisplayUnit](./getdisplayunit/) | Stellt die Einheitenbeschriftung für die angegebene Achse dar. |
| [SetDisplayUnit](./setdisplayunit/) | Stellt die Einheitenbeschriftung für die angegebene Achse dar. |
| [GetCustomDisplayUnit](./getcustomdisplayunit/) | Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |
| [SetCustomDisplayUnit](./setcustomdisplayunit/) | Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |
| [GetDisplayUnitLabel](./getdisplayunitlabel/) | Stellt eine Einheitenbeschriftung auf einer Achse im angegebenen Diagramm dar. Einheitenbeschriftungen sind nützlich, um große Werte zu visualisieren – zum Beispiel in Millionen oder Milliarden. |
| [IsDisplayUnitLabelShown](./isdisplayunitlabelshown/) | Stellt dar, ob die Anzeigeeinheitenbeschriftung auf der angegebenen Achse angezeigt wird. |
| [SetIsDisplayUnitLabelShown](./setisdisplayunitlabelshown/) | Stellt dar, ob die Anzeigeeinheitenbeschriftung auf der angegebenen Achse angezeigt wird. |
| [GetTitle](./gettitle/) | Liefert den Titel dieser Achse im Diagramm. |
| [GetCategoryType](./getcategorytype/) | Stellt den Typ der Kategorienachse dar. |
| [SetCategoryType](./setcategorytype/) | Stellt den Typ der Kategorienachse dar. |
| [GetBaseUnitScale](./getbaseunitscale/) | Stellt die Basiseinheitsskala für die Kategorienachse dar. |
| [SetBaseUnitScale](./setbaseunitscale/) | Stellt die Basiseinheitsskala für die Kategorienachse dar. |
| [GetMajorUnitScale](./getmajorunitscale/) | Stellt die Haupteinheitsskala für die Kategorienachse dar. |
| [SetMajorUnitScale](./setmajorunitscale/) | Stellt die Haupteinheitsskala für die Kategorienachse dar. |
| [GetMinorUnitScale](./getminorunitscale/) | Stellt die Haupteinheitsskala für die Kategorienachse dar. |
| [SetMinorUnitScale](./setminorunitscale/) | Stellt die Haupteinheitsskala für die Kategorienachse dar. |
| [IsVisible](./isvisible/) | Stellt dar, ob die Achse sichtbar ist. |
| [SetIsVisible](./setisvisible/) | Stellt dar, ob die Achse sichtbar ist. |
| [GetMajorGridLines](./getmajorgridlines/) | Stellt die Hauptgitternetzlinien einer Diagrammachse dar. |
| [GetMinorGridLines](./getminorgridlines/) | Stellt die Nebengitternetzlinien einer Diagrammachse dar. |
| [GetHasMultiLevelLabels](./gethasmultilevellabels/) | Gibt an, ob die Beschriftungen mehrstufig angezeigt werden sollen. |
| [SetHasMultiLevelLabels](./sethasmultilevellabels/) | Gibt an, ob die Beschriftungen mehrstufig angezeigt werden sollen. |
| [GetAxisTexts](./getaxistexts/) | Liefert die Beschriftungen der Achse nach Aufruf der Methode Chart.Calculate(). |
| [GetBins](./getbins/) | Stellt Klassen auf einer Diagrammachse (Histogramm/Pareto) dar |
