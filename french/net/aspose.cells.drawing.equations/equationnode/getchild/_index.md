---
title: "EquationNode.GetChild"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode EquationNode. Retourne le nœud à l'index spécifié parmi les enfants du nœud actuel"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnode/getchild/
---
## EquationNode.GetChild method

Renvoie le nœud à l'index spécifié parmi les enfants du nœud actuel.

```csharp
public EquationNode GetChild(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | Index du nœud |

### Valeur de retour

Retourne le nœud correspondant si le nœud spécifié existe, sinon retourne null.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodGetChildWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une forme d'équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Obtenir le paragraphe d'équation et son premier nœud enfant
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Ajouter un nœud délimiteur en tant qu'enfant
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            
            // Ajouter un nœud fraction à l'intérieur du délimiteur
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            FractionEquationNode fractionNode = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);
            
            // Ajouter le numérateur et le dénominateur
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textNode = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textNode.Text = "X";
            
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            textNode = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textNode.Text = "Y";
            
            // Enregistrez le classeur
            workbook.Save("EquationNodeGetChildDemo.xlsx");
            
            // Charger le fichier enregistré pour vérifier
            Workbook loadedWorkbook = new Workbook("EquationNodeGetChildDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Démontrer la méthode GetChild
            EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
            DelimiterEquationNode loadedDelimiter = (DelimiterEquationNode)loadedMathNode.GetChild(0);
            
            Console.WriteLine("Delimiter BeginChar: " + loadedDelimiter.BeginChar);
            Console.WriteLine("Delimiter EndChar: " + loadedDelimiter.EndChar);
            
            EquationNode loadedBaseNode = loadedDelimiter.GetChild(0);
            FractionEquationNode loadedFraction = (FractionEquationNode)loadedBaseNode.GetChild(0);
            
            Console.WriteLine("Fraction node type: " + loadedFraction.EquationType);
        }
    }
}
```

### Voir aussi

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


