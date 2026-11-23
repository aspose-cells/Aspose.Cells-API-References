---
title: "DelimiterEquationNode.BeginChar"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DelimiterEquationNode. Caractère de début du délimiteur"
type: docs
url: /fr/net/aspose.cells.drawing.equations/delimiterequationnode/beginchar/
---
## DelimiterEquationNode.BeginChar property

Caractère de début du délimiteur.

```csharp
public string BeginChar { get; set; }
```

### Remarques

Il convient de noter que cette propriété n'accepte qu'un seul caractère, et si plusieurs caractères sont fournis, seul le premier caractère est accepté.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyBeginCharDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une équation à la première feuille de calcul
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Obtenir le nœud racine de l'équation
            var mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Ajouter un nœud délimiteur avec des caractères de début/fin personnalisés
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.BeginChar = "#";
            delimiterNode.EndChar = "*";
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            
            // Ajouter du contenu à l'intérieur du délimiteur
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Content";
            
            // Enregistrez le classeur
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Workbook saved with custom delimiter equation. BeginChar: " + delimiterNode.BeginChar);
        }
    }
}
```

### Voir aussi

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


