---
title: "GroupCharacterEquationNode.VertJc"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GroupCharacterEquationNode. Questo attributo, combinato con pos di groupChrPr, specifica il layout verticale dell'oggetto groupChr. Dove pos specifica la posizione del carattere di raggruppamento, vertJc specifica l'allineamento dell'oggetto rispetto alla linea di base."
type: docs
url: /it/net/aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/
---
## GroupCharacterEquationNode.VertJc property

Questo attributo, combinato con pos di groupChrPr, specifica la disposizione verticale dell'oggetto groupChr. Dove pos indica la posizione del carattere di raggruppamento, vertJc indica l'allineamento dell'oggetto rispetto alla linea di base.

```csharp
public EquationCharacterPositionType VertJc { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodePropertyVertJcDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma di casella di testo per contenere l'equazione
            var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            
            // Crea un'istanza di GroupCharacterEquationNode
            var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            
            try
            {
                // Imposta le proprietà iniziali per il nodo dell'equazione
                equationNode.GroupChr = "⏟";
                equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
                equationNode.Position = EquationCharacterPositionType.Bottom;
                
                // Dimostra la proprietà VertJc (lettura e scrittura)
                Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
                
                // Modifica il valore di VertJc
                equationNode.VertJc = EquationCharacterPositionType.Top;
                Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
                
                // Salva la cartella di lavoro
                workbook.Save("VertJcDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


