---
title: "Classe MatrixEquationNode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Equations.MatrixEquationNode. Cette classe spécifie l’équation de matrice composée d’un ou plusieurs éléments disposés en une ou plusieurs lignes et en une ou plusieurs colonnes"
type: docs
url: /fr/net/aspose.cells.drawing.equations/matrixequationnode/
---
## MatrixEquationNode class

Cette classe spécifie l'équation Matrix, consistant en un ou plusieurs éléments disposés sur une ou plusieurs lignes et une ou plusieurs colonnes.

```csharp
public class MatrixEquationNode : EquationNode
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BaseJc](../../aspose.cells.drawing.equations/matrixequationnode/basejc/) { get; set; } | Cet attribut spécifie l’alignement de la matrice. Le texte en dehors de la matrice peut être aligné en bas, en haut ou au centre d’une fonction de matrice. Par défaut, la matrice utilise l’alignement centré. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtenez le type d'équation du nœud actuel (hérité de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Renvoie la police de cet objet. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHidePlaceholder](../../aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/) { get; set; } | Cet attribut spécifie la propriété Masquer les espaces réservés sur une matrice. Lorsque cette propriété est activée, les espaces réservés n’apparaissent pas dans la matrice. Par défaut, les espaces réservés apparaissent afin que les emplacements où le texte peut être inséré soient visibles. |
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
| override [Equals](../../aspose.cells.drawing.equations/matrixequationnode/equals/)(object) | Déterminer si le nœud d'équation actuel est égal au nœud spécifié |
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
    public class EquationsClassMatrixEquationNodeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une zone de texte avec équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenir le paragraphe d’équation et ajouter un nœud de matrice
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Définir les propriétés de la matrice
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Ajouter une matrice 2x2 avec des 1 sur la diagonale
            for (int i = 0; i < 2; i++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                for (int j = 0; j < 2; j++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (i == j) ? "1" : "0";
                }
            }

            // Enregistrez le classeur
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);
            Console.WriteLine("Matrix equation created successfully. File saved to: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


