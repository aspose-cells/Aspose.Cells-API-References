---
title: "Class SubSupEquationNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.SubSupEquationNode klass. Denna klass specificerar en ekvation som kan vara upphöjd eller nedsänkt. Det finns fyra huvudformer av denna ekvation: upphöjd, nedsänkt, upphöjd och nedsänkt placerade till vänster om basen samt upphöjd och nedsänkt placerade till höger om basen."
type: docs
url: /sv/net/aspose.cells.drawing.equations/subsupequationnode/
---
## SubSupEquationNode class

Denna klass specificerar en ekvation som valfritt kan vara upphöjd eller nedsänkt. Det finns fyra huvudformer av denna ekvation: upphöjd, nedsänkt, upphöjd och nedsänkt placerade till vänster om basen, samt upphöjd och nedsänkt placerade till höger om basen.

```csharp
public class SubSupEquationNode : EquationNode
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Hämta ekvationstypen för den aktuella noden (ärvd från [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returnerar teckensnittet för detta objekt. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Hämtar längden på tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Anger föräldranoden för den aktuella noden (Ärvt från [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Hämtar startindexet för tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returnerar textalternativen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representerar nodens typ. (Ärvt från [`EquationNode`](../equationnode/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder. (Ärvt från [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/subsupequationnode/equals/)(object) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Returnerar noden på det angivna indexet bland den aktuella nodens barn. (Ärvt från [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Infogar den angivna noden efter den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Infogar den angivna noden före den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens barnnodlista. (Ärvt från [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Tar bort sig själv från föräldern. (Ärvt från [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Tar bort alla barnnoder för den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Tar bort den angivna noden från den aktuella nodens barn. (Ärvt från [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Tar bort noden på det angivna indexet från den aktuella nodens barn. (Ärvt från [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Ställer in den förinställda WordArt‑stilen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Konvertera denna ekvation till ett LaTeX‑uttryck. (Ärvt från [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Konvertera denna ekvation till MathML-uttryck.(Härledd från [`EquationNode`](../equationnode/).) |

### Exempel

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

            // Skapa subekvation (A med subskript B)
            SubSupEquationNode subNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sub);
            AddBaseComponent(subNode, vals[0]);
            AddSubscriptComponent(subNode, vals[1]);

            // Skapa superekvation (A med superskript C)
            SubSupEquationNode supNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sup);
            AddBaseComponent(supNode, vals[0]);
            AddSuperscriptComponent(supNode, vals[2]);

            // Skapa SubSup-ekvation (A med subskript B och superskript C)
            SubSupEquationNode subSupNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.SubSup);
            AddBaseComponent(subSupNode, vals[0]);
            AddSubscriptComponent(subSupNode, vals[1]);
            AddSuperscriptComponent(subSupNode, vals[2]);

            // Skapa PreSubSup-ekvation (subskript B, superskript C, sedan bas A)
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

### Se även

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


