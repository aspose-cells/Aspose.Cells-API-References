---
title: "GroupCharacterEquationNode.VertJc"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GroupCharacterEquationNode. Cet attribut, combiné avec la position de groupChrPr, spécifie la disposition verticale de l'objet groupChr. Où pos indique la position du caractère de groupement, vertJc indique l'alignement de l'objet par rapport à la ligne de base"
type: docs
url: /fr/net/aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/
---
## GroupCharacterEquationNode.VertJc property

Cet attribut, combiné avec le pos de groupChrPr, spécifie la disposition verticale de l'objet groupChr. Là où pos indique la position du caractère de groupement, vertJc indique l'alignement de l'objet par rapport à la ligne de base.

```csharp
public EquationCharacterPositionType VertJc { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme de zone de texte pour contenir l'équation
            var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            
            // Créer une instance de GroupCharacterEquationNode
            var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            
            try
            {
                // Définir les propriétés initiales du nœud d'équation
                equationNode.GroupChr = "⏟";
                equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
                equationNode.Position = EquationCharacterPositionType.Bottom;
                
                // Démontrer la propriété VertJc (lecture et écriture)
                Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
                
                // Modifier la valeur de VertJc
                equationNode.VertJc = EquationCharacterPositionType.Top;
                Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
                
                // Enregistrez le classeur
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

### Voir aussi

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


