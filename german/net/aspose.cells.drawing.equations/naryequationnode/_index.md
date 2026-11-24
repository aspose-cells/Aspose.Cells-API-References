---
title: "Klasse NaryEquationNode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.NaryEquationNode Klasse. Diese Klasse definiert eine n‑stellige Operator‑Gleichung, die aus einem n‑stelligen Operator, einer Basis oder einem Operanden und optionalen oberen und unteren Grenzen besteht."
type: docs
url: /de/net/aspose.cells.drawing.equations/naryequationnode/
---
## NaryEquationNode class

Diese Klasse spezifiziert eine n‑stellige Operator‑Gleichung, die aus einem n‑stelligen Operator, einer Basis (oder Operanden) und optionalen oberen und unteren Grenzen besteht.

```csharp
public class NaryEquationNode : EquationNode
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Erhalte den Gleichungstyp des aktuellen Knotens (geerbt von [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Gibt die Schriftart dieses Objekts zurück. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHideSubscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesubscript/) { get; set; } | Ob die untere Grenze angezeigt werden soll |
| [IsHideSuperscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/) { get; set; } | Ob die obere Grenze angezeigt werden soll |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Liest die Länge der Zeichen. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LimitLocation](../../aspose.cells.drawing.equations/naryequationnode/limitlocation/) { get; set; } | Dieses Attribut gibt die Position der Grenzen bei n-ären Operatoren an. Grenzen können entweder zentriert über und unter dem n-ären Operator liegen oder direkt rechts vom Operator positioniert werden. |
| [NaryGrow](../../aspose.cells.drawing.equations/naryequationnode/narygrow/) { get; set; } | Dieses Attribut legt die Wachstums­eigenschaft von n-ären Operatoren auf Dokumentebene fest. Wenn deaktiviert, wachsen n-äre Operatoren wie Integrale und Summen nicht, um die Höhe ihrer Operanden anzupassen. Wenn aktiviert, wächst der n-äre Operator vertikal, um die Höhe seiner Operanden zu entsprechen. |
| [NaryOperator](../../aspose.cells.drawing.equations/naryequationnode/naryoperator/) { get; set; } | Ein n-ärer Operator, z.B. \"∑\". Es wird dringend empfohlen, das Attribut NaryOperatorType zu verwenden, um den n-ären Operator festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können. |
| [NaryOperatorType](../../aspose.cells.drawing.equations/naryequationnode/naryoperatortype/) { get; set; } | Ein n-ärer Operator, z.B. \"∑\" |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Gibt den übergeordneten Knoten des aktuellen Knotens an (geerbt von [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Liest den Startindex der Zeichen. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Gibt die Textoptionen zurück. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Stellt den Typ des Knotens dar. (Geerbt von [`EquationNode`](../equationnode/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Fügt den angegebenen Knoten am Ende der Kindknotenliste des aktuellen Knotens ein. (Geerbt von [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Fügt einen Knoten des angegebenen Typs am Ende der Kindknotenliste des aktuellen Knotens ein. (Geerbt von [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/naryequationnode/equals/)(object) | Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Gibt den Knoten am angegebenen Index unter den Kindknoten des aktuellen Knotens zurück. (Geerbt von [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Fügt den angegebenen Knoten nach dem aktuellen Knoten ein. (Geerbt von [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Fügt den angegebenen Knoten vor dem aktuellen Knoten ein. (Geerbt von [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Fügt einen Knoten des angegebenen Typs an der angegebenen Indexposition in die Kindknotenliste des aktuellen Knotens ein. (Geerbt von [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Entfernt sich selbst vom übergeordneten Knoten. (Geerbt von [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Entfernt alle Kindknoten des aktuellen Knotens. (Geerbt von [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Entfernt den angegebenen Knoten aus den Kindknoten des aktuellen Knotens. (Geerbt von [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Entfernt den Knoten am angegebenen Index aus den Kindknoten des aktuellen Knotens. (Geerbt von [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Setzt den vordefinierten WordArt-Stil. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Konvertieren Sie diese Gleichung in einen LaTeX-Ausdruck.(Vererbt von [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Konvertieren Sie diese Gleichung in einen MathML-Ausdruck.(Vererbt von [`EquationNode`](../equationnode/).) |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassNaryEquationNodeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Gleichungsform hinzufügen
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Den Gleichungsknoten abrufen
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Einen n-ären Gleichungsknoten erstellen
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // n-äre Eigenschaften festlegen
            naryNode.NaryOperator = "∫";
            naryNode.IsHideSubscript = true;
            naryNode.IsHideSuperscript = true;
            naryNode.NaryGrow = false;

            // Basiskomponente hinzufügen
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";

            // Speichere die Arbeitsmappe
            workbook.Save("NaryEquationDemo.xlsx");

            Console.WriteLine("Nary equation demo created successfully.");
        }
    }
}
```

### Siehe auch

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


