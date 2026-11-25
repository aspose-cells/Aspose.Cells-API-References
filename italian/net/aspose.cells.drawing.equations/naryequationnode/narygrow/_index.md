---
title: "NaryEquationNode.NaryGrow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà NaryEquationNode. Questo attributo specifica la proprietà di crescita degli operatori nari a livello di documento. Quando è disattivata, gli operatori nari come integrali e sommatorie non crescono per corrispondere all'altezza del loro operando. Quando è attivata, l'operatore nario cresce verticalmente per corrispondere all'altezza del suo operando"
type: docs
url: /it/net/aspose.cells.drawing.equations/naryequationnode/narygrow/
---
## NaryEquationNode.NaryGrow property

Questo attributo specifica la proprietà di crescita degli operatori n-ari a livello di documento. Quando disattivata, gli operatori n-ari come integrali e sommatorie non si espandono per corrispondere all'altezza del loro operando. Quando attivata, l'operatore n-ario cresce verticalmente per corrispondere all'altezza dell'operando.

```csharp
public bool NaryGrow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi forma dell'equazione
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Ottieni il nodo dell'equazione
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Crea un nodo operatore nario con la proprietà NaryGrow impostata su true
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            naryNode.NaryOperator = "∑";
            naryNode.NaryGrow = true; // This is the key property we're demonstrating
            
            // Aggiungi pedice (opzionale)
            EquationNode sub = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)sub.AddChild(EquationNodeType.Text);
            subText.Text = "i=1";
            
            // Aggiungi apice (opzionale)
            EquationNode sup = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)sup.AddChild(EquationNodeType.Text);
            supText.Text = "n";
            
            // Aggiungi base (obbligatorio)
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";
            
            // Salva la cartella di lavoro
            workbook.Save("NaryGrowDemo.xlsx");
            
            Console.WriteLine("Equation with NaryGrow property created successfully.");
        }
    }
}
```

### Vedi anche

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


