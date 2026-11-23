---
title: "Énumération EquationLimitLocationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Equations.EquationLimitLocationType enum. Spécifie l'emplacement de la limite sur un opérateur"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationlimitlocationtype/
---
## EquationLimitLocationType enumeration

Spécifie l'emplacement de la limite sur un opérateur.

```csharp
public enum EquationLimitLocationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| UndOvr | `0` | Spécifie que la limite est centrée au-dessus ou en dessous de l'opérateur. |
| SubSup | `1` | Spécifie que la limite se trouve du côté droit de l'opérateur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationLimitLocationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter une forme d'équation à la feuille de calcul
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Obtenir le paragraphe d'équation et son premier enfant
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                // Créer un nœud d'équation Nary
                NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);

                // Définir l'emplacement de la limite sur SubSup (côté droit de l'opérateur)
                naryNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("Limit location set to SubSup: " + naryNode.LimitLocation);

                // Ajouter du contenu à l'équation
                EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
                TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                textNode.Text = "x";

                // Passer à UndOvr (centré au-dessus/en dessous de l'opérateur)
                naryNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("Limit location changed to UndOvr: " + naryNode.LimitLocation);

                // Enregistrez le classeur
                workbook.Save("EquationLimitLocationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


