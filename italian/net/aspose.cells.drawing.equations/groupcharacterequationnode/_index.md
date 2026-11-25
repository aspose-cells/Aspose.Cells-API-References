---
title: "Classe GroupCharacterEquationNode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Equations.GroupCharacterEquationNode. Questa classe specifica la funzione GroupCharacter composta da un carattere disegnato sopra o sotto il testo, spesso con lo scopo di raggruppare visivamente gli elementi."
type: docs
url: /it/net/aspose.cells.drawing.equations/groupcharacterequationnode/
---
## GroupCharacterEquationNode class

Questa classe specifica la funzione Group-Character, costituita da un carattere disegnato sopra o sotto il testo, spesso con lo scopo di raggruppare visivamente gli elementi.

```csharp
public class GroupCharacterEquationNode : EquationNode
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ChrType](../../aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/) { get; set; } | Specifica i caratteri combinanti per valore di tipo. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Ottieni il tipo di equazione del nodo corrente(Ereditato da [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Restituisce il font di questo oggetto.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [GroupChr](../../aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/) { get; set; } | Specifica un simbolo (predefinito U+23DF). Si consiglia vivamente di utilizzare l'attributo ChrType per impostare il carattere di accento. Usa questa impostazione della proprietà se non riesci a trovare il carattere necessario in un tipo noto. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Ottiene la lunghezza dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specifica il nodo genitore del nodo corrente(Ereditato da [`EquationNode`](../equationnode/).) |
| [Position](../../aspose.cells.drawing.equations/groupcharacterequationnode/position/) { get; set; } | Questo attributo specifica la posizione del carattere nell'oggetto |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Ottiene l'indice iniziale dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Restituisce le opzioni di testo.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Rappresenta il tipo del nodo(Ereditato da [`EquationNode`](../equationnode/).) |
| [VertJc](../../aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/) { get; set; } | Questo attributo, combinato con pos di groupChrPr, specifica la disposizione verticale dell'oggetto groupChr. Dove pos indica la posizione del carattere di raggruppamento, vertJc indica l'allineamento dell'oggetto rispetto alla linea di base. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserisce il nodo specificato alla fine dell'elenco dei nodi figlio del nodo corrente(Ereditato da [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/groupcharacterequationnode/equals/)(object) | Determina se il nodo dell'equazione corrente è uguale al nodo specificato |
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
    public class EquationsClassGroupCharacterEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi forma dell'equazione
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Ottieni il nodo matematico e aggiungi il carattere di gruppo
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode groupCharNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Configura le proprietà del carattere di gruppo
            groupCharNode.Position = EquationCharacterPositionType.Top;
            groupCharNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;
            
            // Aggiungi testo di base
            EquationNode baseNode = groupCharNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "abc";
            
            // Salva la cartella di lavoro
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


