---
title: "AccentEquationNode Klasse"
linktitle: "AccentEquationNode"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "AccentEquationNode Klasse. Kapselt das Objekt, das accentequationnode in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/accentequationnode/
---

## AccentEquationNode class

Diese Klasse definiert eine Akzentgleichung, bestehend aus einer Basiskomponente und einem kombinierenden Diakritikum.

```go

type AccentEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewAccentEquationNode](./newaccentequationnode/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetAccentCharacter](./getaccentcharacter/) | Dieses Attribut gibt den Typ des kombinierten diakritischen Zeichens an, das an die Basis der Akzentfunktion angehängt wird. Das Standardakzentzeichen ist U+0302. Es wird dringend empfohlen, das Attribut AccentType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können. |
| [SetAccentCharacter](./setaccentcharacter/) | Dieses Attribut gibt den Typ des kombinierten diakritischen Zeichens an, das an die Basis der Akzentfunktion angehängt wird. Das Standardakzentzeichen ist U+0302. Es wird dringend empfohlen, das Attribut AccentType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können. |
| [GetAccentCharacterType](./getaccentcharactertype/) | Geben Sie kombinierende Zeichen nach Typwert an. |
| [SetAccentCharacterType](./setaccentcharactertype/) | Geben Sie kombinierende Zeichen nach Typwert an. |
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
| [AccentEquationNode_CreateNode](./accentequationnode_createnode/) | Erstelle einen Knoten des angegebenen Typs. |
