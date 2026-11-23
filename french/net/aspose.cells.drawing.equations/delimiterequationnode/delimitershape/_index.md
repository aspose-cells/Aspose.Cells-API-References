---
title: "DelimiterEquationNode.DelimiterShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DelimiterEquationNode. Spécifie la forme des délimiteurs dans l'objet délimiteur"
type: docs
url: /fr/net/aspose.cells.drawing.equations/delimiterequationnode/delimitershape/
---
## DelimiterEquationNode.DelimiterShape property

Spécifie la forme des délimiteurs dans l'objet délimiteur.

```csharp
public EquationDelimiterShapeType DelimiterShape { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyDelimiterShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud d'équation
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Créer un nœud délimiteur avec une forme personnalisée
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";

            // Ajouter du contenu à l'intérieur du délimiteur
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Content";

            // Enregistrez le classeur
            workbook.Save("DelimiterShapeDemo.xlsx");

            Console.WriteLine("Workbook saved with delimiter equation demonstrating DelimiterShape property.");
        }
    }
}
```

### Voir aussi

* enum [EquationDelimiterShapeType](../../equationdelimitershapetype/)
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


