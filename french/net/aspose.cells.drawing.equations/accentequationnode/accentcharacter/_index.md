---
title: "AccentEquationNode.AccentCharacter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AccentEquationNode. Cet attribut spécifie le type de signe diacritique combiné attaché à la base de la fonction d'accent. Le caractère d'accent par défaut est U0302. Il est fortement recommandé d'utiliser l'attribut AccentType pour définir le caractère d'accent. Utilisez ce paramètre de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu."
type: docs
url: /fr/net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

Cet attribut spécifie le type de signe diacritique combiné attaché à la base de la fonction d'accent. Le caractère d'accent par défaut est U+0302. Il est fortement recommandé d'utiliser l'attribut AccentType pour définir le caractère d'accent. Utilisez ce paramètre de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu.

```csharp
public string AccentCharacter { get; set; }
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
    public class AccentEquationNodePropertyAccentCharacterDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une forme d'équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenez le nœud d'équation et ajoutez un nœud d'accent
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            
            // Définissez le caractère d'accent (circonflexe dans ce cas)
            accentNode.AccentCharacter = "\u0302";

            // Ajoutez le texte de base pour l'accent
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "x";

            // Enregistrez le classeur
            workbook.Save("AccentEquationDemo.xlsx");

            // Vérifiez le fichier enregistré en le rechargeant
            Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            // Affichez le caractère d'accent pour démontrer la propriété
            Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
        }
    }
}
```

### Voir aussi

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


