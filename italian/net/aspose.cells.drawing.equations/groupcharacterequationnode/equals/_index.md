---
title: "GroupCharacterEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GroupCharacterEquationNode. Determina se il nodo dell'equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/groupcharacterequationnode/equals/
---
## GroupCharacterEquationNode.Equals method

Determina se il nodo dell'equazione corrente è uguale al nodo specificato

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | Il nodo specificato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due istanze di GroupCharacterEquationNode per il confronto
            // Poiché GroupCharacterEquationNode non ha un costruttore senza parametri,
            // dovremo crearle tramite la ShapeCollection del foglio di lavoro
            var shape1 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node1 = (GroupCharacterEquationNode)shape1.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node1.GroupChr = "⏟";
            node1.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node1.Position = EquationCharacterPositionType.Bottom;
            node1.VertJc = EquationCharacterPositionType.Bottom;

            var shape2 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node2 = (GroupCharacterEquationNode)shape2.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node2.GroupChr = "⏟";
            node2.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node2.Position = EquationCharacterPositionType.Bottom;
            node2.VertJc = EquationCharacterPositionType.Bottom;

            try
            {
                // Chiama il metodo Equals con parametro Object
                bool areEqual = node1.Equals((Object)node2);

                // Visualizza il risultato del confronto
                Console.WriteLine($"The two GroupCharacterEquationNode instances are equal: {areEqual}");

                // Aggiungi il risultato al foglio di lavoro
                worksheet.Cells["A1"].PutValue("GroupCharacterEquationNode Equals Comparison Result:");
                worksheet.Cells["A2"].PutValue(areEqual);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("GroupCharacterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


