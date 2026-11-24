---
title: "Class ArrayEquationNode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.ArrayEquationNode class. Gibt die EquationArray-Funktion an, ein Objekt, das aus einer oder mehreren Gleichungen besteht."
type: docs
url: /de/net/aspose.cells.drawing.equations/arrayequationnode/
---
## ArrayEquationNode class

Definiert die Equation-Array-Funktion, ein Objekt, das aus einer oder mehreren Gleichungen besteht.

```csharp
public class ArrayEquationNode : EquationNode
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
| override [Equals](../../aspose.cells.drawing.equations/arrayequationnode/equals/)(object) | Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist |
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassArrayEquationNodeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Textfeldform hinzu, um die Gleichung zu halten
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 100);

            // Erstelle einen Array-Gleichungs-Knoten (muss mit übergeordnetem Knoten erstellt werden)
            ArrayEquationNode arrayEquation = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);

            // Erstelle einen einfachen Gleichungs-Knoten, um ihn dem Array hinzuzufügen
            // EquationNode ist abstrakt, daher müssen wir einen konkreten Typ erstellen
            // Verwende den Text-Gleichungstyp als einfachste Option
            EquationNode simpleEquation = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation);

            // Füge die einfache Gleichung zur Array-Gleichung hinzu
            arrayEquation.AddChild(simpleEquation);

            // Setze die Gleichung in das Textfeld
            textBox.Text = arrayEquation.ToMathML();

            // Ergebnis speichern
            workbook.Save("ArrayEquationNodeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


