---
title: "Énumération EquationFractionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.Equations.EquationFractionType. Ceci spécifie le style d'affichage de la barre de fraction"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

Cela spécifie le style d'affichage de la barre de fraction.

```csharp
public enum EquationFractionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Bar | `0` | Cela spécifie que le numérateur est au-dessus et le dénominateur en dessous, séparés par une barre au milieu. |
| NoBar | `1` | Cela spécifie que le numérateur est au-dessus et le dénominateur en dessous ne sont pas séparés par une barre au milieu. |
| Linear | `2` | Cela spécifie que le numérateur est à gauche et le dénominateur à droite, séparés par un '/' entre les deux. |
| Skewed | `3` | Cela spécifie que le numérateur est en haut à gauche et le dénominateur en bas à droite, séparés par un \"/\". |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme d'équation
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenez le nœud mathématique et ajoutez une fraction
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
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
            workbook.Save("EquationFractionTypeDemo.xlsx");
            
            Console.WriteLine("Equation with skewed fraction created successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


