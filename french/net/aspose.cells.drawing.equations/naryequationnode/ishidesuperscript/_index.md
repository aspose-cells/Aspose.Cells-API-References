---
title: "NaryEquationNode.IsHideSuperscript"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété NaryEquationNode. Indique s'il faut afficher la borne supérieure"
type: docs
url: /fr/net/aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/
---
## NaryEquationNode.IsHideSuperscript property

Indique si la borne supérieure doit être affichée

```csharp
public bool IsHideSuperscript { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyIsHideSuperscriptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Créer un nœud d'équation Nary avec exposant caché
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSuperscript = true; // Demonstrating the IsHideSuperscript property
            
            // Ajouter le composant de base
            EquationNode baseNode = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";
            
            // Ajouter un exposant (sera caché en raison de IsHideSuperscript = true)
            EquationNode supNode = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)supNode.AddChild(EquationNodeType.Text);
            supText.Text = "2";

            // Enregistrer et recharger pour vérifier que l'exposant est caché
            workbook.Save("NaryEquationDemo.xlsx");
            workbook = new Workbook("NaryEquationDemo.xlsx");
            
            // Vérifier l'équation enregistrée
            TextBox savedTextBox = (TextBox)workbook.Worksheets[0].Shapes[0];
            EquationNode savedMathNode = savedTextBox.GetEquationParagraph().GetChild(0);
            NaryEquationNode savedNode = (NaryEquationNode)savedMathNode.GetChild(0);
            
            Console.WriteLine("Nary Operator: " + savedNode.NaryOperator);
            Console.WriteLine("IsHideSuperscript: " + savedNode.IsHideSuperscript);
            Console.WriteLine("Superscript exists: " + (savedNode.GetChild(1).GetChild(0) != null));
        }
    }
}
```

### Voir aussi

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


