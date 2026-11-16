---
title: "NaryEquationNode Klasse"
linktitle: "NaryEquationNode"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "NaryEquationNode Klasse. Kapselt das Objekt, das naryequationnode in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/naryequationnode/
---

## NaryEquationNode class

Diese Klasse spezifiziert eine n-äre Operator-Gleichung, die aus einem n-ären Operator, einer Basis (oder Operanden) und optionalen oberen und unteren Grenzen besteht.

```go

type NaryEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewNaryEquationNode](./newnaryequationnode/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [IsHideSubscript](./ishidesubscript/) | Ob die untere Grenze angezeigt werden soll |
| [SetIsHideSubscript](./setishidesubscript/) | Ob die untere Grenze angezeigt werden soll |
| [IsHideSuperscript](./ishidesuperscript/) | Ob die obere Grenze angezeigt werden soll |
| [SetIsHideSuperscript](./setishidesuperscript/) | Ob die obere Grenze angezeigt werden soll |
| [GetLimitLocation](./getlimitlocation/) | Dieses Attribut gibt den Ort der Grenzen in n-ären Operatoren an. Grenzen können entweder zentriert über und unter dem n-ären Operator liegen oder direkt rechts vom Operator positioniert werden. |
| [SetLimitLocation](./setlimitlocation/) | Dieses Attribut gibt den Ort der Grenzen in n-ären Operatoren an. Grenzen können entweder zentriert über und unter dem n-ären Operator liegen oder direkt rechts vom Operator positioniert werden. |
| [GetNaryOperator](./getnaryoperator/) | ein n-ärer Operator, z.B. \"∑\". Es wird dringend empfohlen, das Attribut NaryOperatorType zu verwenden, um den n-ären Operator festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können. |
| [SetNaryOperator](./setnaryoperator/) | ein n-ärer Operator, z.B. \"∑\". Es wird dringend empfohlen, das Attribut NaryOperatorType zu verwenden, um den n-ären Operator festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können. |
| [GetNaryOperatorType](./getnaryoperatortype/) | ein n-ärer Operator, z.B. \"∑\" |
| [SetNaryOperatorType](./setnaryoperatortype/) | ein n-ärer Operator, z.B. \"∑\" |
| [GetNaryGrow](./getnarygrow/) | Dieses Attribut legt die Wachstumseigenschaft von n-ären Operatoren auf Dokumentebene fest. Wenn deaktiviert, wachsen n-äre Operatoren wie Integrale und Summen nicht, um die Höhe ihrer Operanden anzupassen. Wenn aktiviert, wächst der n-äre Operator vertikal, um die Höhe seiner Operanden anzupassen. |
| [SetNaryGrow](./setnarygrow/) | Dieses Attribut legt die Wachstumseigenschaft von n-ären Operatoren auf Dokumentebene fest. Wenn deaktiviert, wachsen n-äre Operatoren wie Integrale und Summen nicht, um die Höhe ihrer Operanden anzupassen. Wenn aktiviert, wächst der n-äre Operator vertikal, um die Höhe seiner Operanden anzupassen. |
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
| [NaryEquationNode_CreateNode](./naryequationnode_createnode/) | Erstelle einen Knoten des angegebenen Typs. |
