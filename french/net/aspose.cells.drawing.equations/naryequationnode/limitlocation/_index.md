---
title: "NaryEquationNode.LimitLocation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété NaryEquationNode. Cet attribut spécifie l'emplacement des limites dans les opérateurs n-aires. Les limites peuvent être centrées au-dessus et en dessous de l'opérateur n-aire ou positionnées juste à droite de l'opérateur"
type: docs
url: /fr/net/aspose.cells.drawing.equations/naryequationnode/limitlocation/
---
## NaryEquationNode.LimitLocation property

Cet attribut spécifie l'emplacement des limites dans les opérateurs n-aires. Les limites peuvent être centrées au-dessus et en dessous de l'opérateur n-aire, ou positionnées juste à droite de l'opérateur.

```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyLimitLocationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour contenir l'équation
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Accéder à l'équation et ajouter un nœud d'opérateur n-aire
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Convertir en NaryEquationNode pour accéder à LimitLocation
            var naryEquationNode = (NaryEquationNode)naryNode;

            try
            {
                // Afficher la LimitLocation actuelle (valeur par défaut)
                Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);

                // Définir LimitLocation sur SubSup (limites sur le côté droit)
                naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);

                // Revenir à UndOvr (limites centrées)
                naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);

                // Enregistrez le classeur
                workbook.Save("LimitLocationDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


