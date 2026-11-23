---
title: "TextRunEquationNode.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "TextRunEquationNode propriété. Définir le contenu du nœud texte. Généralement un objet nœud par caractère"
type: docs
url: /fr/net/aspose.cells.drawing.equations/textrunequationnode/text/
---
## TextRunEquationNode.Text property

Définir le contenu du nœud texte (généralement un objet nœud par caractère).

```csharp
public string Text { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class TextRunEquationNodePropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une forme d'équation à la première feuille de calcul
            TextBox textBox = (TextBox)workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud d'équation racine
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Créer une équation fraction
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Ajouter le numérateur avec le texte "X"
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "X";

            // Ajouter le dénominateur avec le texte "Y"
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "Y";

            // Enregistrez le classeur
            workbook.Save("TextRunEquationNodeDemo.xlsx");

            // Vérifiez le fichier enregistré en le rechargeant
            Workbook loadedWorkbook = new Workbook("TextRunEquationNodeDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Accéder aux propriétés du texte pour démontrer la fonctionnalité
            TextRunEquationNode loadedNumeratorText = (TextRunEquationNode)((FractionEquationNode)loadedTextBox
                .GetEquationParagraph()
                .GetChild(0)
                .GetChild(0))
                .GetChild(0)
                .GetChild(0);

            Console.WriteLine("Numerator text: " + loadedNumeratorText.Text);
        }
    }
}
```

### Voir aussi

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


