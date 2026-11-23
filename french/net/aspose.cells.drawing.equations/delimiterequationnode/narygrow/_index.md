---
title: "DelimiterEquationNode.NaryGrow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DelimiterEquationNode. Spécifie si le délimiteur doit s'étendre et se contracter automatiquement avec la hauteur de la formule"
type: docs
url: /fr/net/aspose.cells.drawing.equations/delimiterequationnode/narygrow/
---
## DelimiterEquationNode.NaryGrow property

Spécifie si le délimiteur doit s'étendre et se contracter automatiquement avec la hauteur de la formule.

```csharp
public bool NaryGrow { get; set; }
```

### Remarques

Cette propriété spécifie la propriété de croissance du délimiteur au niveau du document. Lorsqu'elle est désactivée, le délimiteur ne s'agrandit pas pour correspondre à la taille de la hauteur de son composant. Lorsqu'elle est activée, le délimiteur s'étend verticalement pour correspondre à la hauteur de son composant.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            var paragraph = textBox.GetEquationParagraph();
            var mathNode = paragraph.GetChild(0);
            
            // Créer un nœud délimiteur avec la propriété NaryGrow
            var delimiterNode = mathNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Delimiter) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            delimiterNode.DelimiterShape = Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType.Match;
            delimiterNode.NaryGrow = false; // Demonstrating NaryGrow property
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            delimiterNode.SeparatorChar = ",";

            // Ajouter des éléments de base
            var baseNode1 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode1 = baseNode1.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode1.Text = "x";

            var baseNode2 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode2 = baseNode2.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode2.Text = "y";

            // Enregistrer et vérifier
            string outputFile = "DelimiterEquationNode_NaryGrow_Demo.xlsx";
            workbook.Save(outputFile);

            // Vérifier le fichier enregistré
            Workbook verifyWorkbook = new Workbook(outputFile);
            var verifyTextBox = verifyWorkbook.Worksheets[0].Shapes[0] as Aspose.Cells.Drawing.TextBox;
            var verifyNode = verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            
            Console.WriteLine("NaryGrow value: " + verifyNode.NaryGrow); // Should output "False"
        }
    }
}
```

### Voir aussi

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


