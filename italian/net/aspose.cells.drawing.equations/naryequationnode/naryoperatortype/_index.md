---
title: "NaryEquationNode.NaryOperatorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà NaryEquationNode. un operatore nario, ad es."
type: docs
url: /it/net/aspose.cells.drawing.equations/naryequationnode/naryoperatortype/
---
## NaryEquationNode.NaryOperatorType property

un operatore n-ario, ad es. "∑"

```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyNaryOperatorTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per contenere l'equazione
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Accedi all'equazione e aggiungi un nodo operatore nario
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Esegui il cast a NaryEquationNode per accedere a NaryOperatorType
            var naryEquationNode = (NaryEquationNode)naryNode;

            // Mostra il NaryOperatorType corrente (valore predefinito)
            Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);

            // Imposta l'operatore di sommatoria (∑)
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Aggiungi base (operando) e limiti per dimostrare l'operatore
            var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
            var textNode1 = baseNode.AddChild(EquationNodeType.Text);
            textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
            var textNode2 = limitNode.AddChild(EquationNodeType.Text);
            textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var textNode3 = baseNode.AddChild(EquationNodeType.Text);
            textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed

            // Imposta l'operatore affinché cresca con il suo contenuto
            naryEquationNode.NaryGrow = true;

            // Cambia all'operatore prodotto (∏) e mostra la differenza
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            // Salva la cartella di lavoro
            workbook.Save("NaryOperatorTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


