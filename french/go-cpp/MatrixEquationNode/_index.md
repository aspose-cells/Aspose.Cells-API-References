---
title: "Classe MatrixEquationNode"
linktitle: "MatrixEquationNode"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe MatrixEquationNode. Encapsule l'objet qui représente matrixequationnode en Go."
type: docs
weight: 200
url: /fr/go-cpp/matrixequationnode/
---

## MatrixEquationNode class

Cette classe spécifie l'équation de matrice, composée d'un ou plusieurs éléments disposés en une ou plusieurs lignes et en une ou plusieurs colonnes.

```go

type MatrixEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewMatrixEquationNode](./newmatrixequationnode/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetBaseJc](./getbasejc/) | Cet attribut spécifie l'alignement de la matrice. Le texte en dehors de la matrice peut être aligné en bas, en haut ou au centre d'une fonction de matrice. Par défaut, la matrice suppose un alignement centré. |
| [SetBaseJc](./setbasejc/) | Cet attribut spécifie l'alignement de la matrice. Le texte en dehors de la matrice peut être aligné en bas, en haut ou au centre d'une fonction de matrice. Par défaut, la matrice suppose un alignement centré. |
| [IsHidePlaceholder](./ishideplaceholder/) | Cet attribut spécifie la propriété Masquer les espaces réservés sur une matrice. Lorsque cette propriété est activée, les espaces réservés n'apparaissent pas dans la matrice. Par défaut, les espaces réservés apparaissent de sorte que les emplacements où le texte peut être inséré soient visibles. |
| [SetIsHidePlaceholder](./setishideplaceholder/) | Cet attribut spécifie la propriété Masquer les espaces réservés sur une matrice. Lorsque cette propriété est activée, les espaces réservés n'apparaissent pas dans la matrice. Par défaut, les espaces réservés apparaissent de sorte que les emplacements où le texte peut être inséré soient visibles. |
| [Equals](./equals/) | Déterminez si le nœud d'équation actuel est égal au nœud spécifié |
| [GetStartIndex](./getstartindex/) | Obtient l'index de début des caractères. |
| [GetLength](./getlength/) | Obtient la longueur des caractères. |
| [GetFont](./getfont/) | Renvoie la police de cet objet. |
| [SetWordArtStyle](./setwordartstyle/) | Définit le style WordArt prédéfini. |
| [GetTextOptions](./gettextoptions/) | Renvoie les options de texte. |
| [GetType](./gettype/) | Obtient le type du nœud de texte. |
| [GetParentNode](./getparentnode/) | Spécifie le nœud parent du nœud actuel |
| [SetParentNode](./setparentnode/) | Spécifie le nœud parent du nœud actuel |
| [ToLaTeX](./tolatex/) | Convertissez cette équation en expression LaTeX. |
| [ToMathML](./tomathml/) | Convertissez cette équation en expression MathML. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | Insérez un nœud du type spécifié à la fin de la liste des nœuds enfants du nœud actuel. |
| [InsertChild](./insertchild/) | Insère un nœud du type spécifié à la position d'index spécifiée dans la liste des nœuds enfants du nœud actuel. |
| [InsertAfter](./insertafter/) | Insère le nœud spécifié après le nœud actuel. |
| [InsertBefore](./insertbefore/) | Insère le nœud spécifié avant le nœud actuel. |
| [GetChild](./getchild/) | Renvoie le nœud à l'index spécifié parmi les enfants du nœud actuel. |
| [Remove](./remove/) | Supprime lui-même du parent. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | Supprime le nœud spécifié des enfants du nœud actuel. |
| [RemoveAllChildren](./removeallchildren/) | Supprime tous les nœuds enfants du nœud actuel. |
| [GetEquationType](./getequationtype/) | Obtenez le type d'équation du nœud actuel |
| [MatrixEquationNode_CreateNode](./matrixequationnode_createnode/) | Créez un nœud du type spécifié. |
