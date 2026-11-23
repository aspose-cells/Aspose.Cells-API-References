---
title: "Enum EquationDelimiterShapeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType enum. Cela spécifie la forme des délimiteurs dans l'objet délimiteur"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationdelimitershapetype/
---
## EquationDelimiterShapeType enumeration

Cela spécifie la forme des délimiteurs dans l'objet délimiteur.

```csharp
public enum EquationDelimiterShapeType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Centered | `0` | Le séparateur est centré sur toute la hauteur de son contenu. |
| Match | `1` | Le séparateur est ajusté pour correspondre exactement à la hauteur de leurs contenus. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationDelimiterShapeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme d'équation
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Obtenir le nœud d'équation
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Créer un nœud de délimiteur avec le type de forme Match
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "{";
            delimiterNode.EndChar = "}";
            
            // Ajouter du contenu à l'intérieur du délimiteur
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";
            
            // Enregistrez le classeur
            workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


