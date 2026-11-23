---
title: "FractionEquationNode.FractionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FractionEquationNode. Cela spécifie le type de fraction, la valeur par défaut étant Bar"
type: docs
url: /fr/net/aspose.cells.drawing.equations/fractionequationnode/fractiontype/
---
## FractionEquationNode.FractionType property

Cela spécifie le type de fraction ; la valeur par défaut est 'Bar'.

```csharp
public EquationFractionType FractionType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class FractionEquationNodePropertyFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme d'équation
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud mathématique
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Créer un nœud de fraction
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Ajouter le numérateur
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // Ajouter le dénominateur
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // Enregistrer et vérifier
            string outputPath = "FractionEquationDemo.xlsx";
            workbook.Save(outputPath);

            // Recharger pour vérifier
            Workbook verifyWorkbook = new Workbook(outputPath);
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            FractionEquationNode verifyFraction = (FractionEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Fraction Type: " + verifyFraction.FractionType);
            Console.WriteLine("Numerator: " + ((TextRunEquationNode)verifyFraction.GetChild(0).GetChild(0)).Text);
            Console.WriteLine("Denominator: " + ((TextRunEquationNode)verifyFraction.GetChild(1).GetChild(0)).Text);
        }
    }
}
```

### Voir aussi

* enum [EquationFractionType](../../equationfractiontype/)
* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


