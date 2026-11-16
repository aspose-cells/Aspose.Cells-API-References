---
title: "FractionEquationNode Classe"
linktitle: "FractionEquationNode"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "FractionEquationNode classe. Encapsule l'objet qui représente fractionequationnode en Go."
type: docs
weight: 200
url: /fr/go-cpp/fractionequationnode/
---

## FractionEquationNode class

Cette classe spécifie l'équation de fraction, composée d'un numérateur et d'un dénominateur séparés par une barre de fraction. La barre de fraction peut être horizontale ou diagonale, selon les propriétés de la fraction. L'équation de fraction est également utilisée pour représenter la fonction pile, qui place un élément au-dessus d'un autre, sans barre de fraction.

```go

type FractionEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewFractionEquationNode](./newfractionequationnode/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetFractionType](./getfractiontype/) | Cela spécifie le type de fraction ; la valeur par défaut est 'Bar'. |
| [SetFractionType](./setfractiontype/) | Cela spécifie le type de fraction ; la valeur par défaut est 'Bar'. |
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
| [FractionEquationNode_CreateNode](./fractionequationnode_createnode/) | Créez un nœud du type spécifié. |
