---
title: "Classe MathematicalEquationNode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Equations.MathematicalEquationNode. Questa classe specifica un'equazione o un'espressione matematica. Tutto il testo matematico delle equazioni o delle espressioni matematiche è contenuto da questa classe"
type: docs
url: /it/net/aspose.cells.drawing.equations/mathematicalequationnode/
---
## MathematicalEquationNode class

Questa classe specifica un'equazione o un'espressione matematica. Tutto il testo matematico delle equazioni o delle espressioni matematiche è contenuto in questa classe.

```csharp
public class MathematicalEquationNode : EquationNode
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
| override [Equals](../../aspose.cells.drawing.equations/mathematicalequationnode/equals/)(object) | Determina se il nodo dell'equazione corrente è uguale al nodo specificato |
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassMathematicalEquationNodeDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook per la dimostrazione
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Crea due istanze di MathematicalEquationNode per il confronto
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;

                // Dimostrare il metodo Equals
                bool areEqual = node1?.Equals((object)node2) ?? false;
                Console.WriteLine($"MathematicalEquationNode comparison result: {areEqual}");

                // Salva la cartella di lavoro
                workbook.Save("MathematicalEquationNodeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MathematicalEquationNode: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


