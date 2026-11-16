---
title: "MatrixEquationNode-Klasse"
linktitle: "MatrixEquationNode"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "MatrixEquationNode-Klasse. Kapselt das Objekt, das matrixequationnode in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/matrixequationnode/
---

## MatrixEquationNode class

Diese Klasse spezifiziert die Matrixgleichung, die aus einem oder mehreren Elementen besteht, die in ein oder mehrere Zeilen und ein oder mehrere Spalten angeordnet sind.

```go

type MatrixEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewMatrixEquationNode](./newmatrixequationnode/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetBaseJc](./getbasejc/) | Dieses Attribut gibt die Ausrichtung der Matrix an. Text außerhalb der Matrix kann am unteren, oberen oder mittleren Teil einer Matrixfunktion ausgerichtet werden. Standardmäßig nimmt die Matrix die mittlere Ausrichtung an. |
| [SetBaseJc](./setbasejc/) | Dieses Attribut gibt die Ausrichtung der Matrix an. Text außerhalb der Matrix kann am unteren, oberen oder mittleren Teil einer Matrixfunktion ausgerichtet werden. Standardmäßig nimmt die Matrix die mittlere Ausrichtung an. |
| [IsHidePlaceholder](./ishideplaceholder/) | Dieses Attribut legt die Eigenschaft Hide Placeholders für eine Matrix fest. Wenn diese Eigenschaft aktiviert ist, erscheinen Platzhalter nicht in der Matrix. Standardmäßig erscheinen Platzhalter, sodass die Stellen, an denen Text eingefügt werden kann, sichtbar werden. |
| [SetIsHidePlaceholder](./setishideplaceholder/) | Dieses Attribut legt die Eigenschaft Hide Placeholders für eine Matrix fest. Wenn diese Eigenschaft aktiviert ist, erscheinen Platzhalter nicht in der Matrix. Standardmäßig erscheinen Platzhalter, sodass die Stellen, an denen Text eingefügt werden kann, sichtbar werden. |
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
| [MatrixEquationNode_CreateNode](./matrixequationnode_createnode/) | Erstelle einen Knoten des angegebenen Typs. |
