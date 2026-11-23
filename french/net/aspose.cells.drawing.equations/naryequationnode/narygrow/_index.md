---
title: "NaryEquationNode.NaryGrow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "NaryEquationNode propriété. Cet attribut spécifie la propriété de croissance des opérateurs n-aires au niveau du document. Lorsqu'elle est désactivée, les opérateurs n-aires tels que les intégrales et les sommes ne s'agrandissent pas pour correspondre à la hauteur de leur opérande. Lorsqu'elle est activée, l'opérateur n-aire s'étend verticalement pour correspondre à la hauteur de son opérande"
type: docs
url: /fr/net/aspose.cells.drawing.equations/naryequationnode/narygrow/
---
## NaryEquationNode.NaryGrow property

Cet attribut spécifie la propriété de croissance des opérateurs n-aires au niveau du document. Lorsqu'il est désactivé, les opérateurs n-aires tels que les intégrales et les sommes ne s'agrandissent pas pour correspondre à la hauteur de leur opérande. Lorsqu'il est activé, l'opérateur n-aire s'agrandit verticalement pour correspondre à la hauteur de son opérande.

```csharp
public bool NaryGrow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme d'équation
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Obtenir le nœud d'équation
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Créer un nœud d'opérateur n-aire avec la propriété NaryGrow définie sur true
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            naryNode.NaryOperator = "∑";
            naryNode.NaryGrow = true; // This is the key property we're demonstrating
            
            // Ajouter un indice (facultatif)
            EquationNode sub = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)sub.AddChild(EquationNodeType.Text);
            subText.Text = "i=1";
            
            // Ajouter un exposant (facultatif)
            EquationNode sup = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)sup.AddChild(EquationNodeType.Text);
            supText.Text = "n";
            
            // Ajouter la base (obligatoire)
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";
            
            // Enregistrez le classeur
            workbook.Save("NaryGrowDemo.xlsx");
            
            Console.WriteLine("Equation with NaryGrow property created successfully.");
        }
    }
}
```

### Voir aussi

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


