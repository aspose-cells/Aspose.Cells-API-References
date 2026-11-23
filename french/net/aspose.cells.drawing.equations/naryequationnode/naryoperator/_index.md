---
title: "NaryEquationNode.NaryOperator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété NaryEquationNode. un opérateur n-aire, par ex. Il est fortement recommandé d'utiliser l'attribut NaryOperatorType pour définir l'opérateur n-aire. Utilisez ce paramètre de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu"
type: docs
url: /fr/net/aspose.cells.drawing.equations/naryequationnode/naryoperator/
---
## NaryEquationNode.NaryOperator property

un opérateur n-aire, p. \"∑\". Il est fortement recommandé d'utiliser l'attribut NaryOperatorType pour définir l'opérateur n-aire. Utilisez ce paramètre de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu.

```csharp
public string NaryOperator { get; set; }
```

### Remarques

Il convient de noter que cette propriété n'accepte qu'un seul caractère, et si plusieurs caractères sont fournis, seul le premier caractère est accepté.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryOperatorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'équation
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud d'équation
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Créer un nœud d'opérateur n-aire
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Définir les propriétés de l'opérateur n-aire
            naryNode.NaryOperator = "\u2211"; // Summation symbol
            naryNode.NaryGrow = true;

            // Ajouter un indice (facultatif)
            EquationNode subscript = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subscriptText = (TextRunEquationNode)subscript.AddChild(EquationNodeType.Text);
            subscriptText.Text = "i=1";

            // Ajouter un exposant (facultatif)
            EquationNode superscript = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscript.AddChild(EquationNodeType.Text);
            superscriptText.Text = "n";

            // Ajouter l'expression de base
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";

            // Enregistrez le classeur
            workbook.Save("NaryOperatorDemo.xlsx");

            Console.WriteLine("Nary operator equation created successfully.");
        }
    }
}
```

### Voir aussi

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


