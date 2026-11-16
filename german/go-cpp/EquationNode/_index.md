---
title: "EquationNode Klasse"
linktitle: "EquationNode"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "EquationNode Klasse. Kapselt das Objekt, das equationnode in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/equationnode/
---

## EquationNode class

Abstrakte Klasse zum Ableiten anderer Gleichungsknoten.

```go

type EquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewEquationNode](./newequationnode/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetParentNode](./getparentnode/) | Gibt den übergeordneten Knoten des aktuellen Knotens an. |
| [SetParentNode](./setparentnode/) | Gibt den übergeordneten Knoten des aktuellen Knotens an. |
| [ToLaTeX](./tolatex/) | Konvertiere diese Gleichung in einen LaTeX‑Ausdruck. |
| [ToMathML](./tomathml/) | Konvertiere diese Gleichung in einen MathML‑Ausdruck. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | Füge einen Knoten des angegebenen Typs am Ende der Kindknotenliste des aktuellen Knotens ein. |
| [AddChild_EquationNode](./addchild_equationnode/) | Fügt den angegebenen Knoten am Ende der Kindknotenliste des aktuellen Knotens ein. |
| [InsertChild](./insertchild/) | Fügt einen Knoten des angegebenen Typs an der angegebenen Indexposition in der Kindknotenliste des aktuellen Knotens ein. |
| [InsertAfter](./insertafter/) | Fügt den angegebenen Knoten nach dem aktuellen Knoten ein. |
| [InsertBefore](./insertbefore/) | Fügt den angegebenen Knoten vor dem aktuellen Knoten ein. |
| [GetChild](./getchild/) | Gibt den Knoten am angegebenen Index unter den Kindknoten des aktuellen Knotens zurück. |
| [Remove](./remove/) | Entfernt sich selbst vom übergeordneten Element. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | Entfernt den angegebenen Knoten aus den Kindknoten des aktuellen Knotens. |
| [RemoveChild_Int](./removechild_int/) | Entfernt den Knoten am angegebenen Index aus den Kindknoten des aktuellen Knotens. |
| [RemoveAllChildren](./removeallchildren/) | Entfernt alle Kindknoten des aktuellen Knotens. |
| [Equals](./equals/) | Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist |
| [GetType](./gettype/) | Stellt den Typ des Knotens dar. |
| [GetEquationType](./getequationtype/) | Erhalte den Gleichungstyp des aktuellen Knotens |
| [EquationNode_CreateNode](./equationnode_createnode/) | Erstelle einen Knoten des angegebenen Typs. |
| [GetStartIndex](./getstartindex/) | Ermittelt den Startindex der Zeichen. |
| [GetLength](./getlength/) | Ermittelt die Länge der Zeichen. |
| [GetFont](./getfont/) | Gibt die Schriftart dieses Objekts zurück. |
| [SetWordArtStyle](./setwordartstyle/) | Setzt den voreingestellten WordArt‑Stil. |
| [GetTextOptions](./gettextoptions/) | Gibt die Textoptionen zurück. |
