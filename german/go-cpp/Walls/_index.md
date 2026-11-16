---
title: "Wände Klasse"
linktitle: "Wände"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Wände Klasse. Kapselt das Objekt, das Wände in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/walls/
---

## Walls class

Kapselt das Objekt, das die Wände eines 3‑D‑Diagramms darstellt.

```go

type Walls struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewWalls](./newwalls/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetCenterX](./getcenterx/) | Gibt die x‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammbreite zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetCenterY](./getcentery/) | Gibt die y‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammhöhe zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetWidth](./getwidth/) | Gibt die Breite von links nach rechts in Einheiten von 1/4000 der Diagrammbreite zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetDepth](./getdepth/) | Gibt die Tiefe von vorne nach hinten in Einheiten von 1/4000 der Diagrammbreite zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetHeight](./getheight/) | Gibt die Höhe von oben nach unten in Einheiten von 1/4000 der Diagrammhöhe zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetCenterXPx](./getcenterxpx/) | Gibt die x‑Koordinate der linken unteren Ecke des Wandzentrums in Pixeln zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetCenterYPx](./getcenterypx/) | Gibt die y‑Koordinate der linken unteren Ecke des Wandzentrums in Pixeln zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetWidthPx](./getwidthpx/) | Gibt die Breite von links nach rechts in Pixeln zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetDepthPx](./getdepthpx/) | Gibt die Tiefe von vorne nach hinten in Pixeln zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetHeightPx](./getheightpx/) | Gibt die Höhe von oben nach unten in Pixeln zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetCubePointCount](./getcubepointcount/) | Gibt die Anzahl der Würfelpunkte zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetCubePointXPx](./getcubepointxpx/) | Gibt die x‑Koordinate des Scheitelpunkts des Wandwürfels zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. Die Anzahl der Scheitelpunkte des Wandwürfels beträgt acht. |
| [GetCubePointYPx](./getcubepointypx/) | Gibt die y‑Koordinate des Scheitelpunkts des Wandwürfels zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde. Die Anzahl der Scheitelpunkte des Wandwürfels beträgt acht. |
| [GetBackgroundColor](./getbackgroundcolor/) | Liest oder setzt die Hintergrundfarbe des Bereichs. |
| [SetBackgroundColor](./setbackgroundcolor/) | Liest oder setzt die Hintergrundfarbe des Bereichs. |
| [GetForegroundColor](./getforegroundcolor/) | Liest oder setzt die Vordergrundfarbe. |
| [SetForegroundColor](./setforegroundcolor/) | Liest oder setzt die Vordergrundfarbe. |
| [GetFormatting](./getformatting/) | Stellt die Formatierung des Bereichs dar. |
| [SetFormatting](./setformatting/) | Stellt die Formatierung des Bereichs dar. |
| [GetInvertIfNegative](./getinvertifnegative/) | Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden die Vordergrundfarbe und die Hintergrundfarbe vertauscht. |
| [SetInvertIfNegative](./setinvertifnegative/) | Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden die Vordergrundfarbe und die Hintergrundfarbe vertauscht. |
| [GetFillFormat](./getfillformat/) | Stellt ein FillFormat-Objekt dar, das Füllformatierungs‑Eigenschaften für das angegebene Diagramm oder die angegebene Form enthält. |
| [GetTransparency](./gettransparency/) | Gibt den Transparenzgrad des Bereichs zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (klar). |
| [SetTransparency](./settransparency/) | Gibt den Transparenzgrad des Bereichs zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (klar). |
| [GetBorder](./getborder/) | Liest oder setzt die Randlinie. |
| [SetBorder](./setborder/) | Liest oder setzt die Randlinie. |
