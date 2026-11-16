---
title: "Trendline Klasse"
linktitle: "Trendline"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Trendline Klasse. Kapselt das Objekt, das trendline in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/trendline/
---

## Trendline class

Stellt eine Trendlinie in einem Diagramm dar.

```go

type Trendline struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewTrendline](./newtrendline/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [IsNameAuto](./isnameauto/) | Gibt zurück, ob Microsoft Excel den Namen der Trendlinie automatisch bestimmt. |
| [SetIsNameAuto](./setisnameauto/) | Gibt zurück, ob Microsoft Excel den Namen der Trendlinie automatisch bestimmt. |
| [GetType](./gettype/) | Gibt den Trendlinientyp zurück. |
| [GetName](./getname/) | Gibt den Namen der Trendlinie zurück. |
| [SetName](./setname/) | Gibt den Namen der Trendlinie zurück. |
| [GetOrder](./getorder/) | Gibt die Trendlinienreihenfolge zurück oder setzt sie (eine ganze Zahl größer als 1), wenn der Trendlinientyp Polynomisch ist. Die Reihenfolge muss zwischen 2 und 6 liegen. |
| [SetOrder](./setorder/) | Gibt die Trendlinienreihenfolge zurück oder setzt sie (eine ganze Zahl größer als 1), wenn der Trendlinientyp Polynomisch ist. Die Reihenfolge muss zwischen 2 und 6 liegen. |
| [GetPeriod](./getperiod/) | Gibt den Zeitraum für die gleitende Mittelwert‑Trendlinie zurück oder setzt ihn. |
| [SetPeriod](./setperiod/) | Gibt den Zeitraum für die gleitende Mittelwert‑Trendlinie zurück oder setzt ihn. |
| [GetForward](./getforward/) | Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück, über die die Trendlinie nach vorne verläuft, oder setzt sie. Die Anzahl der Perioden muss größer oder gleich null sein. |
| [SetForward](./setforward/) | Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück, über die die Trendlinie nach vorne verläuft, oder setzt sie. Die Anzahl der Perioden muss größer oder gleich null sein. |
| [GetBackward](./getbackward/) | Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück, über die die Trendlinie nach hinten verläuft, oder setzt sie. Die Anzahl der Perioden muss größer oder gleich null sein. Wenn der Diagrammtyp Säule ist, muss die Anzahl der Perioden zwischen 0 und 0,5 liegen. |
| [SetBackward](./setbackward/) | Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück, über die die Trendlinie nach hinten verläuft, oder setzt sie. Die Anzahl der Perioden muss größer oder gleich null sein. Wenn der Diagrammtyp Säule ist, muss die Anzahl der Perioden zwischen 0 und 0,5 liegen. |
| [GetDisplayEquation](./getdisplayequation/) | Gibt an, ob die Gleichung der Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftungsfeld wie der R‑Quadrat‑Wert). Das Setzen dieser Eigenschaft auf True schaltet automatisch Datenbeschriftungen ein. |
| [SetDisplayEquation](./setdisplayequation/) | Gibt an, ob die Gleichung der Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftungsfeld wie der R‑Quadrat‑Wert). Das Setzen dieser Eigenschaft auf True schaltet automatisch Datenbeschriftungen ein. |
| [GetDisplayRSquared](./getdisplayrsquared/) | Gibt an, ob der R‑Quadrat‑Wert der Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftungsfeld wie die Gleichung). Das Setzen dieser Eigenschaft auf True schaltet automatisch Datenbeschriftungen ein. |
| [SetDisplayRSquared](./setdisplayrsquared/) | Gibt an, ob der R‑Quadrat‑Wert der Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftungsfeld wie die Gleichung). Das Setzen dieser Eigenschaft auf True schaltet automatisch Datenbeschriftungen ein. |
| [GetIntercept](./getintercept/) | Gibt den Punkt zurück, an dem die Trendlinie die Werteachse schneidet, oder setzt ihn. |
| [SetIntercept](./setintercept/) | Gibt den Punkt zurück, an dem die Trendlinie die Werteachse schneidet, oder setzt ihn. |
| [GetDataLabels](./getdatalabels/) | Stellt das DataLabels‑Objekt für die angegebene Serie dar. |
| [GetLegendEntry](./getlegendentry/) | Liest den Legendeintrag gemäß dieser Trendlinie. |
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
