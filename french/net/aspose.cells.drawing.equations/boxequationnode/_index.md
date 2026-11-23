---
title: "Classe BoxEquationNode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Equations.BoxEquationNode. Cette classe spécifie la fonction boîte qui est utilisée pour regrouper les composants d'une équation"
type: docs
url: /fr/net/aspose.cells.drawing.equations/boxequationnode/
---
## BoxEquationNode class

Cette classe spécifie la fonction box, qui est utilisée pour regrouper les composants d'une équation.

```csharp
public class BoxEquationNode : EquationNode
```

## Propriétés

| Nom | Description |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtenez le type d'équation du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Renvoie la police de cet objet. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtient la longueur des caractères. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Spécifie le nœud parent du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtient l'index de départ des caractères. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Renvoie les options de texte. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Représente le type du nœud (hérité de [`EquationNode`](../equationnode/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Insère le nœud spécifié à la fin de la liste des nœuds enfants du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insérer un nœud du type spécifié à la fin de la liste des nœuds enfants du nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/boxequationnode/equals/)(object) | Déterminer si le nœud d'équation actuel est égal au nœud spécifié |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Renvoie le nœud à l'index spécifié parmi les enfants du nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Insère le nœud spécifié après le nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Insère le nœud spécifié avant le nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Insère un nœud du type spécifié à la position d'index spécifiée dans la liste des nœuds enfants du nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Se supprime du parent.(Hérité de [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Supprime tous les nœuds enfants du nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Supprime le nœud spécifié des enfants du nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Supprime le nœud à l'index spécifié des enfants du nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Définit le style WordArt prédéfini.(Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Convertir cette équation en expression LaTeX.(Hérité de [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Convertir cette équation en expression MathML.(Hérité de [`EquationNode`](../equationnode/).) |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassBoxEquationNodeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez une zone de texte d'équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenez le nœud d'équation depuis la zone de texte
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Ajoutez un nœud d'équation Box
            BoxEquationNode boxNode = (BoxEquationNode)mathNode.AddChild(EquationNodeType.Box);
            
            // Ajoutez un nœud de base à la boîte
            EquationNode baseNode = boxNode.AddChild(EquationNodeType.Base);
            
            // Ajoutez du texte au nœud de base
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "==";

            // Enregistrez le classeur
            string outputFile = "BoxEquationDemo.xlsx";
            workbook.Save(outputFile);

            Console.WriteLine("Equation with Box node created successfully. File saved to: " + outputFile);
        }
    }
}
```

### Voir aussi

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


