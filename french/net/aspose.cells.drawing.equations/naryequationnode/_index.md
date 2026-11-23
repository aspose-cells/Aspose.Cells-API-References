---
title: "Classe NaryEquationNode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Equations.NaryEquationNode class. Cette classe spécifie une équation d'opérateur n-aire composée d'un opérateur n-aire, d'une base ou d'un opérande et de limites supérieures et inférieures facultatives"
type: docs
url: /fr/net/aspose.cells.drawing.equations/naryequationnode/
---
## NaryEquationNode class

Cette classe spécifie une équation d'opérateur n-aire consistant en un opérateur n-aire, une base (ou opérande), et des bornes supérieures et inférieures optionnelles.

```csharp
public class NaryEquationNode : EquationNode
```

## Propriétés

| Nom | Description |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtenez le type d'équation du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Renvoie la police de cet objet. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHideSubscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesubscript/) { get; set; } | Indique si la borne inférieure doit être affichée |
| [IsHideSuperscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/) { get; set; } | Indique si la borne supérieure doit être affichée |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtient la longueur des caractères. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LimitLocation](../../aspose.cells.drawing.equations/naryequationnode/limitlocation/) { get; set; } | Cet attribut spécifie l'emplacement des limites dans les opérateurs n-aires. Les limites peuvent être centrées au-dessus et en dessous de l'opérateur n-aire, ou positionnées juste à droite de l'opérateur. |
| [NaryGrow](../../aspose.cells.drawing.equations/naryequationnode/narygrow/) { get; set; } | Cet attribut spécifie la propriété de croissance des opérateurs n-aires au niveau du document. Lorsqu'il est désactivé, les opérateurs n-aires tels que les intégrales et les sommes ne s'agrandissent pas pour correspondre à la hauteur de leur opérande. Lorsqu'il est activé, l'opérateur n-aire s'agrandit verticalement pour correspondre à la hauteur de son opérande. |
| [NaryOperator](../../aspose.cells.drawing.equations/naryequationnode/naryoperator/) { get; set; } | un opérateur n-aire, p. \"∑\". Il est fortement recommandé d'utiliser l'attribut NaryOperatorType pour définir l'opérateur n-aire. Utilisez ce paramètre de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu. |
| [NaryOperatorType](../../aspose.cells.drawing.equations/naryequationnode/naryoperatortype/) { get; set; } | un opérateur n-aire, p. \"∑\" |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Spécifie le nœud parent du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtient l'index de départ des caractères. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Renvoie les options de texte. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Représente le type du nœud (hérité de [`EquationNode`](../equationnode/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Insère le nœud spécifié à la fin de la liste des nœuds enfants du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insérer un nœud du type spécifié à la fin de la liste des nœuds enfants du nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/naryequationnode/equals/)(object) | Déterminer si le nœud d'équation actuel est égal au nœud spécifié |
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
    public class EquationsClassNaryEquationNodeDemo
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

            // Créer un nœud d'équation n-aire
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Définir les propriétés n-aires
            naryNode.NaryOperator = "∫";
            naryNode.IsHideSubscript = true;
            naryNode.IsHideSuperscript = true;
            naryNode.NaryGrow = false;

            // Ajouter le composant de base
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";

            // Enregistrez le classeur
            workbook.Save("NaryEquationDemo.xlsx");

            Console.WriteLine("Nary equation demo created successfully.");
        }
    }
}
```

### Voir aussi

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


