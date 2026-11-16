---
title: "DelimiterEquationNode Klasse"
linktitle: "DelimiterEquationNode"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DelimiterEquationNode Klasse. Kapselt das Objekt, das delimiterequationnode in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/delimiterequationnode/
---

## DelimiterEquationNode class

Diese Klasse spezifiziert die Delimiter-Gleichung, die aus öffnenden und schließenden Begrenzungszeichen (wie Klammern, geschweiften Klammern, eckigen Klammern und senkrechten Strichen) und einer darin enthaltenen Komponente besteht. Der Delimiter kann mehr als eine Komponente haben, mit einem festgelegten Trennzeichen zwischen den einzelnen Komponenten.

```go

type DelimiterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewDelimiterEquationNode](./newdelimiterequationnode/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetBeginChar](./getbeginchar/) | Anfangszeichen des Trennzeichens. |
| [SetBeginChar](./setbeginchar/) | Anfangszeichen des Trennzeichens. |
| [GetEndChar](./getendchar/) | Endzeichen des Trennzeichens. |
| [SetEndChar](./setendchar/) | Endzeichen des Trennzeichens. |
| [GetNaryGrow](./getnarygrow/) | Gibt an, ob das Trennzeichen automatisch mit der Höhe der Formel erweitert und verkleinert werden soll. |
| [SetNaryGrow](./setnarygrow/) | Gibt an, ob das Trennzeichen automatisch mit der Höhe der Formel erweitert und verkleinert werden soll. |
| [GetSeparatorChar](./getseparatorchar/) | Trennzeichen‑Trennzeichen‑Zeichen. |
| [SetSeparatorChar](./setseparatorchar/) | Trennzeichen‑Trennzeichen‑Zeichen. |
| [GetDelimiterShape](./getdelimitershape/) | Gibt die Form der Trennzeichen im Trennzeichenobjekt an. |
| [SetDelimiterShape](./setdelimitershape/) | Gibt die Form der Trennzeichen im Trennzeichenobjekt an. |
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
| [DelimiterEquationNode_CreateNode](./delimiterequationnode_createnode/) | Erstelle einen Knoten des angegebenen Typs. |
