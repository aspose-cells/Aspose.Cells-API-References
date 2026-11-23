---
title: "EquationNodeParagraph.Justification"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété EquationNodeParagraph. Cela spécifie l'alignement du paragraphe mathématique, une série d'équations adjacentes dans le même paragraphe. Un paragraphe mathématique peut être Aligné à gauche, Aligné à droite, Centré ou Centré en groupe. Par défaut, le paragraphe mathématique est Centré en groupe. Cela signifie que les équations peuvent être alignées les unes par rapport aux autres, mais que l'ensemble du groupe d'équations est centré dans son ensemble"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnodeparagraph/justification/
---
## EquationNodeParagraph.Justification property

Cela spécifie l'alignement du paragraphe mathématique (une série d'équations adjacentes au sein du même paragraphe). Un paragraphe mathématique peut être aligné à gauche, aligné à droite, centré, ou centré en groupe. Par défaut, le paragraphe mathématique est centré en groupe. Cela signifie que les équations peuvent être alignées les unes par rapport aux autres, mais que l'ensemble du groupe d'équations est centré dans son ensemble.

```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphPropertyJustificationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour contenir l'équation
            var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

            // Obtenir le paragraphe d'équation
            var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

            // Afficher la valeur d'alignement actuelle
            Console.WriteLine("Current Justification value: " + equationParagraph.Justification);

            // Définir différentes valeurs d'alignement et observer les effets
            equationParagraph.Justification = EquationHorizontalJustificationType.Left;
            Console.WriteLine("Set to Left justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Center;
            Console.WriteLine("Set to Center justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
            Console.WriteLine("Set to CenterGroup justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Right;
            Console.WriteLine("Set to Right justification");

            // Enregistrez le classeur
            workbook.Save("EquationJustificationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


