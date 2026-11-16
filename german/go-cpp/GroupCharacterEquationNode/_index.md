---
title: "GroupCharacterEquationNode-Klasse"
linktitle: "GroupCharacterEquationNode"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "GroupCharacterEquationNode-Klasse. Kapselt das Objekt, das groupcharacterequationnode in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/groupcharacterequationnode/
---

## GroupCharacterEquationNode class

Diese Klasse spezifiziert die Group-Character-Funktion, die aus einem Zeichen besteht, das über oder unter Text gesetzt wird, häufig mit dem Zweck, Elemente visuell zu gruppieren.

```go

type GroupCharacterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewGroupCharacterEquationNode](./newgroupcharacterequationnode/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetGroupChr](./getgroupchr/) | Gibt ein Symbol an (Standard U+23DF). Es wird dringend empfohlen, das Attribut ChrType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können. |
| [SetGroupChr](./setgroupchr/) | Gibt ein Symbol an (Standard U+23DF). Es wird dringend empfohlen, das Attribut ChrType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können. |
| [GetChrType](./getchrtype/) | Geben Sie kombinierende Zeichen nach Typwert an. |
| [SetChrType](./setchrtype/) | Geben Sie kombinierende Zeichen nach Typwert an. |
| [GetPosition](./getposition/) | Dieses Attribut gibt die Position des Zeichens im Objekt an. |
| [SetPosition](./setposition/) | Dieses Attribut gibt die Position des Zeichens im Objekt an. |
| [GetVertJc](./getvertjc/) | Dieses Attribut gibt zusammen mit pos von groupChrPr das vertikale Layout des groupChr-Objekts an. Dabei gibt pos die Position des Gruppierungszeichens an, vertJc gibt die Ausrichtung des Objekts relativ zur Grundlinie an. |
| [SetVertJc](./setvertjc/) | Dieses Attribut gibt zusammen mit pos von groupChrPr das vertikale Layout des groupChr-Objekts an. Dabei gibt pos die Position des Gruppierungszeichens an, vertJc gibt die Ausrichtung des Objekts relativ zur Grundlinie an. |
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
| [GroupCharacterEquationNode_CreateNode](./groupcharacterequationnode_createnode/) | Erstelle einen Knoten des angegebenen Typs. |
