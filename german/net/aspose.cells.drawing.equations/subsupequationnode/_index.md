---
title: "Class SubSupEquationNode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.SubSupEquationNode class. Diese Klasse spezifiziert eine Gleichung, die optional hoch- oder tiefgestellt sein kann. Es gibt vier Hauptformen dieser Gleichung: Hochstellung, Tiefstellung, Hochstellung und Tiefstellung, wobei die Hoch- bzw. Tiefstellung links vom Basiszeichen bzw. rechts vom Basiszeichen platziert wird."
type: docs
url: /de/net/aspose.cells.drawing.equations/subsupequationnode/
---
## SubSupEquationNode class

Diese Klasse spezifiziert eine Gleichung, die optional als Hoch- oder Tiefstellung dargestellt werden kann. Es gibt vier Hauptformen dieser Gleichung: Hochstellung, Tiefstellung, Hoch‑ und Tiefstellung links von der Basis sowie Hoch‑ und Tiefstellung rechts von der Basis.

```csharp
public class SubSupEquationNode : EquationNode
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Erhalte den Gleichungstyp des aktuellen Knotens (geerbt von [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Gibt die Schriftart dieses Objekts zurück. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Liest die Länge der Zeichen. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Gibt den übergeordneten Knoten des aktuellen Knotens an (geerbt von [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Liest den Startindex der Zeichen. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Gibt die Textoptionen zurück. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Stellt den Typ des Knotens dar. (Geerbt von [`EquationNode`](../equationnode/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Fügt den angegebenen Knoten am Ende der Kindknotenliste des aktuellen Knotens ein. (Geerbt von [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Fügt einen Knoten des angegebenen Typs am Ende der Kindknotenliste des aktuellen Knotens ein. (Geerbt von [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/subsupequationnode/equals/)(object) | Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist |
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
    public class EquationsClassSubSupEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            string[] vals = new string[] { "A", "B", "C" };

            // Erstelle Sub-Gleichung (A mit Tiefstellung B)
            SubSupEquationNode subNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sub);
            AddBaseComponent(subNode, vals[0]);
            AddSubscriptComponent(subNode, vals[1]);

            // Erstelle Sup-Gleichung (A mit Hochstellung C)
            SubSupEquationNode supNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sup);
            AddBaseComponent(supNode, vals[0]);
            AddSuperscriptComponent(supNode, vals[2]);

            // Erstelle SubSup-Gleichung (A mit Tiefstellung B und Hochstellung C)
            SubSupEquationNode subSupNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.SubSup);
            AddBaseComponent(subSupNode, vals[0]);
            AddSubscriptComponent(subSupNode, vals[1]);
            AddSuperscriptComponent(subSupNode, vals[2]);

            // Erstelle PreSubSup-Gleichung (Tiefstellung B, Hochstellung C, dann Basis A)
            SubSupEquationNode preSubSupNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.PreSubSup);
            AddSubscriptComponent(preSubSupNode, vals[1]);
            AddSuperscriptComponent(preSubSupNode, vals[2]);
            AddBaseComponent(preSubSupNode, vals[0]);

            workbook.Save("SubSupEquationDemo.xlsx");
        }

        private static void AddBaseComponent(SubSupEquationNode parent, string text)
        {
            EquationNode baseNode = parent.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = text;
        }

        private static void AddSubscriptComponent(SubSupEquationNode parent, string text)
        {
            EquationNode subNode = parent.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode textNode = (TextRunEquationNode)subNode.AddChild(EquationNodeType.Text);
            textNode.Text = text;
        }

        private static void AddSuperscriptComponent(SubSupEquationNode parent, string text)
        {
            EquationNode supNode = parent.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode textNode = (TextRunEquationNode)supNode.AddChild(EquationNodeType.Text);
            textNode.Text = text;
        }
    }
}
```

### Siehe auch

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


