---
title: "Classe SubSupEquationNode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Equations.SubSupEquationNode. Questa classe specifica un'equazione che può essere opzionalmente in apice o in pedice. Esistono quattro forme principali di questa equazione: apice, pedice, apice e pedice posizionati a sinistra della base, e apice e pedice posizionati a destra della base."
type: docs
url: /it/net/aspose.cells.drawing.equations/subsupequationnode/
---
## SubSupEquationNode class

Questa classe specifica un'equazione che può essere opzionalmente in apice o in pedice. Esistono quattro forme principali di questa equazione: apice, pedice, apice e pedice posizionati a sinistra della base, apice e pedice posizionati a destra della base.

```csharp
public class SubSupEquationNode : EquationNode
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Ottieni il tipo di equazione del nodo corrente(Ereditato da [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Restituisce il font di questo oggetto.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Ottiene la lunghezza dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specifica il nodo genitore del nodo corrente(Ereditato da [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Ottiene l'indice iniziale dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Restituisce le opzioni di testo.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Rappresenta il tipo del nodo(Ereditato da [`EquationNode`](../equationnode/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserisce il nodo specificato alla fine dell'elenco dei nodi figlio del nodo corrente(Ereditato da [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/subsupequationnode/equals/)(object) | Determina se il nodo dell'equazione corrente è uguale al nodo specificato |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Restituisce il nodo all'indice specificato tra i figli del nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Inserisce il nodo specificato dopo il nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Inserisce il nodo specificato prima del nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Inserisce un nodo del tipo specificato nella posizione di indice specificato nell'elenco dei nodi figlio del nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Rimuove se stesso dal genitore.(Ereditato da [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Rimuove tutti i nodi figlio del nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Rimuove il nodo specificato dai figli del nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Rimuove il nodo all'indice specificato dai figli del nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Imposta lo stile WordArt predefinito.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Converti questa equazione in espressione LaTeX.(Ereditato da [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Converti questa equazione in espressione MathML.(Ereditato da [`EquationNode`](../equationnode/).) |

### Esempi

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

            // Crea equazione Sub (A con pedice B)
            SubSupEquationNode subNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sub);
            AddBaseComponent(subNode, vals[0]);
            AddSubscriptComponent(subNode, vals[1]);

            // Crea equazione Sup (A con apice C)
            SubSupEquationNode supNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sup);
            AddBaseComponent(supNode, vals[0]);
            AddSuperscriptComponent(supNode, vals[2]);

            // Crea equazione SubSup (A con pedice B e apice C)
            SubSupEquationNode subSupNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.SubSup);
            AddBaseComponent(subSupNode, vals[0]);
            AddSubscriptComponent(subSupNode, vals[1]);
            AddSuperscriptComponent(subSupNode, vals[2]);

            // Crea equazione PreSubSup (pedice B, apice C, poi base A)
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

### Vedi anche

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


