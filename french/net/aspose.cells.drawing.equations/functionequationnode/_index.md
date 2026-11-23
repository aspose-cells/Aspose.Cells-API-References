---
title: "Classe FunctionEquationNode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Equations.FunctionEquationNode classe. Cette classe spécifie l'équation FunctionApply qui se compose d'un nom de fonction et d'un argument appliqué. Les types des composants nom et argument sont EquationNodeType.FunctionName et EquationNodeType.Base respectivement."
type: docs
url: /fr/net/aspose.cells.drawing.equations/functionequationnode/
---
## FunctionEquationNode class

Cette classe spécifie l'équation Function-Apply, qui consiste en un nom de fonction et un argument sur lequel on agit. Les types des composants nom et argument sont 'EquationNodeType.FunctionName' et 'EquationNodeType.Base' respectivement.

```csharp
public class FunctionEquationNode : EquationNode
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
| override [Equals](../../aspose.cells.drawing.equations/functionequationnode/equals/)(object) | Déterminer si le nœud d'équation actuel est égal au nœud spécifié |
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
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassFunctionEquationNodeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une équation à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud racine de l'équation
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Créer un nœud de fonction avec un nom en exposant
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
            EquationNode baseArg = functionNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode argText = (TextRunEquationNode)baseArg.AddChild(EquationNodeType.Text);
            argText.Text = "x";

            // Enregistrez le classeur
            workbook.Save("FunctionEquationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


