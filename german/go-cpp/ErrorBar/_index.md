---
title: "ErrorBar-Klasse"
linktitle: "ErrorBar"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ErrorBar-Klasse. Kapselt das Objekt, das den ErrorBar in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/errorbar/
---

## ErrorBar class

Stellt den Fehlerbalken einer Datenserie dar.

```go

type ErrorBar struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewErrorBar](./newerrorbar/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetType](./gettype/) | Stellt den Betragstyp der Fehlermarge dar. |
| [SetType](./settype/) | Stellt den Betragstyp der Fehlermarge dar. |
| [GetDisplayType](./getdisplaytype/) | Stellt den Anzeigetyp des ErrorBar dar. |
| [SetDisplayType](./setdisplaytype/) | Stellt den Anzeigetyp des ErrorBar dar. |
| [GetAmount](./getamount/) | Stellt die Menge des ErrorBar dar. |
| [SetAmount](./setamount/) | Stellt die Menge des ErrorBar dar. |
| [GetShowMarkerTTop](./getshowmarkerttop/) | Gibt an, ob Fehlerbalken mit einem T-Oben formatiert werden. |
| [SetShowMarkerTTop](./setshowmarkerttop/) | Gibt an, ob Fehlerbalken mit einem T-Oben formatiert werden. |
| [GetPlusValue](./getplusvalue/) | Stellt den positiven Fehlerbetrag dar, wenn der ErrorBar-Typ Custom ist. |
| [SetPlusValue](./setplusvalue/) | Stellt den positiven Fehlerbetrag dar, wenn der ErrorBar-Typ Custom ist. |
| [GetMinusValue](./getminusvalue/) | Stellt den negativen Fehlbetrag dar, wenn der Fehlbalkentyp Custom ist. |
| [SetMinusValue](./setminusvalue/) | Stellt den negativen Fehlbetrag dar, wenn der Fehlbalkentyp Custom ist. |
| [GetCompoundType](./getcompoundtype/) | Gibt den zusammengesetzten Linientyp an |
| [SetCompoundType](./setcompoundtype/) | Gibt den zusammengesetzten Linientyp an |
| [GetDashType](./getdashtype/) | Gibt den Strichlinientyp an |
| [SetDashType](./setdashtype/) | Gibt den Strichlinientyp an |
| [GetCapType](./getcaptype/) | Gibt die Endkappen an. |
| [SetCapType](./setcaptype/) | Gibt die Endkappen an. |
| [GetJoinType](./getjointype/) | Gibt die Verbindungskappen an. |
| [SetJoinType](./setjointype/) | Gibt die Verbindungskappen an. |
| [GetBeginType](./getbegintype/) | Gibt eine Pfeilspitze für den Anfang einer Linie an. |
| [SetBeginType](./setbegintype/) | Gibt eine Pfeilspitze für den Anfang einer Linie an. |
| [GetEndType](./getendtype/) | Gibt eine Pfeilspitze für das Ende einer Linie an. |
| [SetEndType](./setendtype/) | Gibt eine Pfeilspitze für das Ende einer Linie an. |
| [GetBeginArrowLength](./getbeginarrowlength/) | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an. |
| [SetBeginArrowLength](./setbeginarrowlength/) | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an. |
| [GetEndArrowLength](./getendarrowlength/) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [SetEndArrowLength](./setendarrowlength/) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [GetBeginArrowWidth](./getbeginarrowwidth/) | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an. |
| [SetBeginArrowWidth](./setbeginarrowwidth/) | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an. |
| [GetEndArrowWidth](./getendarrowwidth/) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [SetEndArrowWidth](./setendarrowwidth/) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [GetThemeColor](./getthemecolor/) | Liest und setzt die Themenfarbe. |
| [SetThemeColor](./setthemecolor/) | Liest und setzt die Themenfarbe. |
| [GetColor](./getcolor/) | Stellt die Farbe der Linie dar. |
| [SetColor](./setcolor/) | Stellt die Farbe der Linie dar. |
| [GetTransparency](./gettransparency/) | Gibt den Transparenzgrad der Linie zurück oder setzt ihn als Wert von 0.0 (undurchsichtig) bis 1.0 (transparent). |
| [SetTransparency](./settransparency/) | Gibt den Transparenzgrad der Linie zurück oder setzt ihn als Wert von 0.0 (undurchsichtig) bis 1.0 (transparent). |
| [GetStyle](./getstyle/) | Stellt den Stil der Linie dar. |
| [SetStyle](./setstyle/) | Stellt den Stil der Linie dar. |
| [GetWeight](./getweight/) | Liest oder setzt den WeightType der Linie. |
| [SetWeight](./setweight/) | Liest oder setzt den WeightType der Linie. |
| [GetWeightPt](./getweightpt/) | Liest oder setzt das Gewicht der Linie in Punkten. |
| [SetWeightPt](./setweightpt/) | Liest oder setzt das Gewicht der Linie in Punkten. |
| [GetWeightPx](./getweightpx/) | Liest oder setzt das Gewicht der Linie in Pixeln. |
| [SetWeightPx](./setweightpx/) | Liest oder setzt das Gewicht der Linie in Pixeln. |
| [GetFormattingType](./getformattingtype/) | Liest oder setzt den Formattyp. |
| [SetFormattingType](./setformattingtype/) | Liest oder setzt den Formattyp. |
| [IsAutomaticColor](./isautomaticcolor/) | Gibt an, ob die Farbe der Linie automatisch zugewiesen wird. |
| [IsVisible](./isvisible/) | Stellt dar, ob die Linie sichtbar ist. |
| [SetIsVisible](./setisvisible/) | Stellt dar, ob die Linie sichtbar ist. |
| [IsAuto](./isauto/) | Gibt an, ob dieser Linienstil automatisch zugewiesen ist. |
| [SetIsAuto](./setisauto/) | Gibt an, ob dieser Linienstil automatisch zugewiesen ist. |
| [GetGradientFill](./getgradientfill/) | Stellt einen Farbverlauf dar. |
