---
title: "Klasse FractionEquationNode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.FractionEquationNode Klasse. Diese Klasse definiert die Bruchgleichung, die aus einem Zähler und einem Nenner besteht, die durch einen Bruchstrich getrennt sind. Der Bruchstrich kann je nach Bruch‑Eigenschaften horizontal oder diagonal sein. Die Bruchgleichung wird auch verwendet, um die Stapelfunktion darzustellen, die ein Element über einem anderen ohne Bruchstrich platziert."
type: docs
url: /de/net/aspose.cells.drawing.equations/fractionequationnode/
---
## FractionEquationNode class

Diese Klasse definiert die Bruchgleichung, bestehend aus einem Zähler und einem Nenner, getrennt durch einen Bruchstrich. Der Bruchstrich kann horizontal oder diagonal sein, abhängig von den Bruch‑Eigenschaften. Die Bruchgleichung wird auch verwendet, um die Stapel‑Funktion darzustellen, bei der ein Element über einem anderen platziert wird, ohne Bruchstrich.

```csharp
public class FractionEquationNode : EquationNode
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Erhalte den Gleichungstyp des aktuellen Knotens (geerbt von [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Gibt die Schriftart dieses Objekts zurück. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FractionType](../../aspose.cells.drawing.equations/fractionequationnode/fractiontype/) { get; set; } | Dies gibt den Typ des Bruchs an; standardmäßig ist 'Bar'. |
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
| override [Equals](../../aspose.cells.drawing.equations/fractionequationnode/equals/)(object) | Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist |
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
    public class EquationsClassFractionEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gleichungs-Textfeld hinzufügen
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Bruchgleichung erstellen
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Zähler hinzufügen
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // Nenner hinzufügen
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // Speichere die Arbeitsmappe
            workbook.Save("FractionEquationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


