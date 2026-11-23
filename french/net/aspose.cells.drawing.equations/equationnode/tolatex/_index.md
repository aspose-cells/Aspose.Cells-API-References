---
title: "EquationNode.ToLaTeX"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode EquationNode. Convertit cette équation en expression LaTeX"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnode/tolatex/
---
## EquationNode.ToLaTeX method

Convertir cette équation en expression LaTeX.

```csharp
public string ToLaTeX()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToLaTeXDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour contenir l'équation
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Obtenir le nœud d'équation
            var equationNode = shape.GetEquationParagraph();

            // Créer une équation fraction simple
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "1";
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "2";

            try
            {
                // Appeler la méthode ToLaTeX
                string latexExpression = equationNode.ToLaTeX();
                
                // Afficher le résultat
                Console.WriteLine("LaTeX expression: " + latexExpression);
                
                // Ajouter la sortie LaTeX à une cellule
                worksheet.Cells["A1"].PutValue("LaTeX Output:");
                worksheet.Cells["B1"].PutValue(latexExpression);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToLaTeX method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("EquationToLaTeXDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


