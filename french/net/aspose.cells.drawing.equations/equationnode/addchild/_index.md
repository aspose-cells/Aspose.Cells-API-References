---
title: "EquationNode.AddChild"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "EquationNode méthode. Insérer un nœud du type spécifié à la fin de la liste des nœuds enfants du nœud actuel"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnode/addchild/
---
## AddChild(EquationNodeType) {#addchild}

Insérer un nœud du type spécifié à la fin de la liste des nœuds enfants du nœud actuel.

```csharp
public EquationNode AddChild(EquationNodeType equationType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| equationType | EquationNodeType | Types de nœuds d'équation |

### Valeur de retour

Si le type spécifié existe, le nœud correspondant est renvoyé, et si le type n'existe pas, un nœud de type inconnu est renvoyé.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodAddChildWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une forme d'équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud mathématique racine
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Créer un nœud fonction et ajouter des enfants
            FunctionEquationNode functionNode = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);
            
            // Ajouter le nom de fonction avec un exposant
            EquationNode functionName = functionNode.AddChild(EquationNodeType.FunctionName);
            EquationNode supNode = functionName.AddChild(EquationNodeType.Sup);
            
            // Ajouter le texte de base pour le nom de la fonction
            EquationNode baseNode = supNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "Add";
            
            // Ajouter du texte en exposant
            EquationNode superscriptNode = supNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscriptNode.AddChild(EquationNodeType.Text);
            superscriptText.Text = "-2";
            
            // Ajouter un argument de fonction
            EquationNode argumentNode = functionNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode argumentText = (TextRunEquationNode)argumentNode.AddChild(EquationNodeType.Text);
            argumentText.Text = "x";

            // Enregistrez le classeur
            workbook.Save("EquationNodeAddChildDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## AddChild(EquationNode) {#addchild_1}

Insère le nœud spécifié à la fin de la liste des nœuds enfants du nœud actuel.

```csharp
public void AddChild(EquationNode node)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nœud | EquationNode | Le nœud spécifié |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodAddChildWithEquationNodeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme d'équation
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Créer un nœud texte pour servir de parent
                var parentNode = equationNode.AddChild(EquationNodeType.Text);
                if (parentNode is TextRunEquationNode textNode)
                {
                    textNode.Text = "Parent Text";
                }

                // Créer un nœud enfant à ajouter en utilisant la méthode statique CreateNode
                var childNode = EquationNode.CreateNode(EquationNodeType.Text, workbook, null);
                if (childNode is TextRunEquationNode childTextNode)
                {
                    childTextNode.Text = "Child Text";
                }

                // Appeler la méthode AddChild avec le paramètre EquationNode
                parentNode.AddChild(childNode);

                Console.WriteLine("AddChild method called successfully with EquationNode parameter");
                Console.WriteLine("Parent node has children: " + (parentNode.GetChild(0) != null));

                // Enregistrez le classeur
                workbook.Save("EquationNodeAddChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling AddChild: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


