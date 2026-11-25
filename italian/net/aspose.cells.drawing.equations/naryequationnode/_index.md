---
title: "Class NaryEquationNode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Equations.NaryEquationNode class. Questa classe specifica un'equazione con operatore n-ario composta da un operatore n-ario, una base o operando e limiti superiori e inferiori opzionali"
type: docs
url: /it/net/aspose.cells.drawing.equations/naryequationnode/
---
## NaryEquationNode class

Questa classe specifica un'equazione operatore n-ario composta da un operatore n-ario, una base (o operando) e limiti superiori e inferiori opzionali.

```csharp
public class NaryEquationNode : EquationNode
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Ottieni il tipo di equazione del nodo corrente(Ereditato da [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Restituisce il font di questo oggetto.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHideSubscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesubscript/) { get; set; } | Indica se visualizzare il limite inferiore |
| [IsHideSuperscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/) { get; set; } | Indica se visualizzare il limite superiore |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Ottiene la lunghezza dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LimitLocation](../../aspose.cells.drawing.equations/naryequationnode/limitlocation/) { get; set; } | Questo attributo specifica la posizione dei limiti negli operatori n-ari. I limiti possono essere centrati sopra e sotto l'operatore n-ario, oppure posizionati appena a destra dell'operatore. |
| [NaryGrow](../../aspose.cells.drawing.equations/naryequationnode/narygrow/) { get; set; } | Questo attributo specifica la proprietà di crescita degli operatori n-ari a livello di documento. Quando disattivata, gli operatori n-ari come integrali e sommatorie non si espandono per corrispondere all'altezza del loro operando. Quando attivata, l'operatore n-ario cresce verticalmente per corrispondere all'altezza dell'operando. |
| [NaryOperator](../../aspose.cells.drawing.equations/naryequationnode/naryoperator/) { get; set; } | un operatore n-ario, ad es. "∑". Si raccomanda vivamente di utilizzare l'attributo NaryOperatorType per impostare l'operatore n-ario. Usa questa impostazione di proprietà se non riesci a trovare il carattere necessario in un tipo conosciuto. |
| [NaryOperatorType](../../aspose.cells.drawing.equations/naryequationnode/naryoperatortype/) { get; set; } | un operatore n-ario, ad es. "∑" |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specifica il nodo genitore del nodo corrente(Ereditato da [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Ottiene l'indice iniziale dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Restituisce le opzioni di testo.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Rappresenta il tipo del nodo(Ereditato da [`EquationNode`](../equationnode/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserisce il nodo specificato alla fine dell'elenco dei nodi figlio del nodo corrente(Ereditato da [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente.(Ereditato da [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/naryequationnode/equals/)(object) | Determina se il nodo dell'equazione corrente è uguale al nodo specificato |
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
    public class EquationsClassNaryEquationNodeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di equazione
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo dell'equazione
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crea un nodo di equazione n-ario
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Imposta le proprietà n-arie
            naryNode.NaryOperator = "∫";
            naryNode.IsHideSubscript = true;
            naryNode.IsHideSuperscript = true;
            naryNode.NaryGrow = false;

            // Aggiungi componente di base
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";

            // Salva la cartella di lavoro
            workbook.Save("NaryEquationDemo.xlsx");

            Console.WriteLine("Nary equation demo created successfully.");
        }
    }
}
```

### Vedi anche

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


