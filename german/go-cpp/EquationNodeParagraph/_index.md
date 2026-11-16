---
title: "EquationNodeParagraph Klasse"
linktitle: "EquationNodeParagraph"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "EquationNodeParagraph Klasse. Kapselt das Objekt, das equationnodeparagraph in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/equationnodeparagraph/
---

## EquationNodeParagraph class

Diese Klasse spezifiziert einen mathematischen Absatz, der ein oder mehrere MathEquationNode(OMath)-Elemente enthält.

```go

type EquationNodeParagraph struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewEquationNodeParagraph](./newequationnodeparagraph/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetJustification](./getjustification/) | Dies gibt die Ausrichtung des mathematischen Absatzes an (eine Reihe benachbarter Gleichungen innerhalb desselben Absatzes). Ein mathematischer Absatz kann linksbündig, rechtsbündig, zentriert oder als Gruppe zentriert sein. Standardmäßig ist der mathematische Absatz als Gruppe zentriert. Das bedeutet, dass die Gleichungen zueinander ausgerichtet werden können, aber die gesamte Gruppe von Gleichungen als Ganzes zentriert ist. |
| [SetJustification](./setjustification/) | Dies gibt die Ausrichtung des mathematischen Absatzes an (eine Reihe benachbarter Gleichungen innerhalb desselben Absatzes). Ein mathematischer Absatz kann linksbündig, rechtsbündig, zentriert oder als Gruppe zentriert sein. Standardmäßig ist der mathematische Absatz als Gruppe zentriert. Das bedeutet, dass die Gleichungen zueinander ausgerichtet werden können, aber die gesamte Gruppe von Gleichungen als Ganzes zentriert ist. |
| [Equals](./equals/) | Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist |
| [GetStartIndex](./getstartindex/) | Ermittelt den Startindex der Zeichen. |
| [GetLength](./getlength/) | Ermittelt die Länge der Zeichen. |
| [GetFont](./getfont/) | Gibt die Schriftart dieses Objekts zurück. |
| [SetWordArtStyle](./setwordartstyle/) | Setzt den voreingestellten WordArt‑Stil. |
| [GetTextOptions](./gettextoptions/) | Gibt die Textoptionen zurück. |
| [GetType](./gettype/) | Liest den Typ des Textknotens. |
| [GetParentNode](./getparentnode/) | Gibt den übergeordneten Knoten des aktuellen Knotens an. |
| [SetParentNode](./setparentnode/) | Gibt den übergeordneten Knoten des aktuellen Knotens an. |
| [ToLaTeX](./tolatex/) | Konvertiere diese Gleichung in einen LaTeX‑Ausdruck. |
| [ToMathML](./tomathml/) | Konvertiere diese Gleichung in einen MathML‑Ausdruck. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | Füge einen Knoten des angegebenen Typs am Ende der Kindknotenliste des aktuellen Knotens ein. |
| [InsertChild](./insertchild/) | Fügt einen Knoten des angegebenen Typs an der angegebenen Indexposition in der Kindknotenliste des aktuellen Knotens ein. |
| [InsertAfter](./insertafter/) | Fügt den angegebenen Knoten nach dem aktuellen Knoten ein. |
| [InsertBefore](./insertbefore/) | Fügt den angegebenen Knoten vor dem aktuellen Knoten ein. |
| [GetChild](./getchild/) | Gibt den Knoten am angegebenen Index unter den Kindknoten des aktuellen Knotens zurück. |
| [Remove](./remove/) | Entfernt sich selbst vom übergeordneten Element. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | Entfernt den angegebenen Knoten aus den Kindknoten des aktuellen Knotens. |
| [RemoveAllChildren](./removeallchildren/) | Entfernt alle Kindknoten des aktuellen Knotens. |
| [GetEquationType](./getequationtype/) | Erhalte den Gleichungstyp des aktuellen Knotens |
| [EquationNodeParagraph_CreateNode](./equationnodeparagraph_createnode/) | Erstelle einen Knoten des angegebenen Typs. |
