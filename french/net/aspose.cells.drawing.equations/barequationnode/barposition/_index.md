---
title: "BarEquationNode.BarPosition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BarEquationNode. Cet attribut spécifie la position de la barre dans l'objet barre"
type: docs
url: /fr/net/aspose.cells.drawing.equations/barequationnode/barposition/
---
## BarEquationNode.BarPosition property

Cet attribut spécifie la position de la barre dans l'objet barre

```csharp
public EquationCharacterPositionType BarPosition { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class BarEquationNodePropertyBarPositionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une forme d'équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud d'équation
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Créer un nœud d'équation de barre
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            
            // Définir la position de la barre sur Haut
            barNode.BarPosition = EquationCharacterPositionType.Top;

            // Ajouter le contenu de base pour la barre
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Enregistrez le classeur
            workbook.Save("BarEquationDemo.xlsx");

            // Vérifier le fichier enregistré
            Workbook verifyWorkbook = new Workbook("BarEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode verifyBarNode = (BarEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + verifyBarNode.BarPosition);
            Console.WriteLine("Base Content: " + ((TextRunEquationNode)verifyBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Voir aussi

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


