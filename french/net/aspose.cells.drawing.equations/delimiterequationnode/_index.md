---
title: "Classe DelimiterEquationNode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Equations.DelimiterEquationNode classe. Cette classe spécifie l'équation de délimiteur composée de délimiteurs ouvrants et fermants tels que les parenthèses, accolades, crochets et barres verticales ainsi qu'un composant contenu à l'intérieur. Le délimiteur peut comporter plusieurs composants avec un caractère séparateur désigné entre chaque composant."
type: docs
url: /fr/net/aspose.cells.drawing.equations/delimiterequationnode/
---
## DelimiterEquationNode class

Cette classe spécifie l'équation délimiteur, composée de délimiteurs ouvrants et fermants (tels que parenthèses, accolades, crochets et barres verticales), ainsi qu'un composant contenu à l'intérieur. Le délimiteur peut contenir plusieurs composants, avec un caractère séparateur désigné entre chaque composant.

```csharp
public class DelimiterEquationNode : EquationNode
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BeginChar](../../aspose.cells.drawing.equations/delimiterequationnode/beginchar/) { get; set; } | Caractère de début du délimiteur. |
| [DelimiterShape](../../aspose.cells.drawing.equations/delimiterequationnode/delimitershape/) { get; set; } | Spécifie la forme des délimiteurs dans l'objet délimiteur. |
| [EndChar](../../aspose.cells.drawing.equations/delimiterequationnode/endchar/) { get; set; } | Caractère de fin du délimiteur. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtenez le type d'équation du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Renvoie la police de cet objet. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtient la longueur des caractères. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [NaryGrow](../../aspose.cells.drawing.equations/delimiterequationnode/narygrow/) { get; set; } | Spécifie si le délimiteur doit s'étendre et se contracter automatiquement avec la hauteur de la formule. |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Spécifie le nœud parent du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [SeparatorChar](../../aspose.cells.drawing.equations/delimiterequationnode/separatorchar/) { get; set; } | Caractère séparateur du délimiteur. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtient l'index de départ des caractères. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Renvoie les options de texte. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Représente le type du nœud (hérité de [`EquationNode`](../equationnode/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Insère le nœud spécifié à la fin de la liste des nœuds enfants du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insérer un nœud du type spécifié à la fin de la liste des nœuds enfants du nœud actuel.(Hérité de [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/delimiterequationnode/equals/)(object) | Déterminer si le nœud d'équation actuel est égal au nœud spécifié |
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
    public class EquationsClassDelimiterEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Créer un nœud de délimiteur avec des paramètres personnalisés
            DelimiterEquationNode node = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            node.DelimiterShape = EquationDelimiterShapeType.Match;
            node.NaryGrow = false;
            node.SeparatorChar = "!";
            node.BeginChar = "#";
            node.EndChar = "*";

            // Ajouter une fraction comme contenu de base
            EquationNode baseNode = node.AddChild(EquationNodeType.Base);
            FractionEquationNode fraction = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);

            // Ajouter le numérateur
            EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textRun = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textRun.Text = "A";

            // Ajouter le dénominateur
            EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
            textRun = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textRun.Text = "B";

            // Ajouter un autre nœud de base avec du texte
            baseNode = node.AddChild(EquationNodeType.Base);
            textRun = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textRun.Text = "a";

            // Enregistrez le classeur
            workbook.Save("DelimiterEquationNodeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


