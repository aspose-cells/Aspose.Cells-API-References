---
title: "Classe EquationNode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Equations.EquationNode. Classe astratta per derivare altri nodi di equazione"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/
---
## EquationNode class

Classe astratta per derivare altri nodi di equazione.

```csharp
public abstract class EquationNode : FontSetting
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Ottieni il tipo di equazione del nodo corrente |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Restituisce il font di questo oggetto.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Ottiene la lunghezza dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specifica il nodo genitore del nodo corrente |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Ottiene l'indice iniziale dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Restituisce le opzioni di testo.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Rappresenta il tipo del nodo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateNode](../../aspose.cells.drawing.equations/equationnode/createnode/)(EquationNodeType, Workbook, EquationNode) | Crea un nodo del tipo specificato. |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild_1)(EquationNode) | Inserisce il nodo specificato alla fine dell'elenco dei nodi figlio del nodo corrente. |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild)(EquationNodeType) | Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente. |
| override [Equals](../../aspose.cells.drawing.equations/equationnode/equals/)(object) | Determina se il nodo dell'equazione corrente è uguale al nodo specificato |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Restituisce il nodo all'indice specificato tra i figli del nodo corrente. |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Inserisce il nodo specificato dopo il nodo corrente. |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Inserisce il nodo specificato prima del nodo corrente. |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Inserisce un nodo del tipo specificato nella posizione di indice specificata nell'elenco dei nodi figlio del nodo corrente. |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Rimuove se stesso dal genitore. |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Rimuove tutti i nodi figlio del nodo corrente. |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild)(EquationNode) | Rimuove il nodo specificato dai figli del nodo corrente. |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild_1)(int) | Rimuove il nodo all'indice specificato dai figli del nodo corrente. |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Imposta lo stile WordArt predefinito.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Converti questa equazione in espressione LaTeX. |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Converti questa equazione in espressione MathML. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationNodeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una casella di testo al foglio di lavoro e ottieni il suo indice.
            int textBoxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "=A1+B1";
            
            // Ottieni il nodo di equazione dalla casella di testo.
            EquationNode node = textBox.GetEquationParagraph();
            
            // Restituisci il testo dell'equazione usando ToString()
            Console.WriteLine("Equation: " + node.ToString());
            
            // Modifica l'equazione impostando un nuovo testo.
            textBox.Text = "=A1*B1";
            Console.WriteLine("Modified Equation: " + textBox.Text);
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


