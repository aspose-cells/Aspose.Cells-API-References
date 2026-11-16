---
title: "EquationNodeParagraph Classe"
linktitle: "EquationNodeParagraph"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "EquationNodeParagraph classe. Encapsule l'objet qui représente equationnodeparagraph en Go."
type: docs
weight: 200
url: /fr/go-cpp/equationnodeparagraph/
---

## EquationNodeParagraph class

Cette classe spécifie un paragraphe mathématique contenant un ou plusieurs éléments MathEquationNode(OMath).

```go

type EquationNodeParagraph struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewEquationNodeParagraph](./newequationnodeparagraph/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetJustification](./getjustification/) | Cela spécifie l'alignement du paragraphe mathématique (une série d'équations adjacentes au sein du même paragraphe). Un paragraphe mathématique peut être aligné à gauche, aligné à droite, centré, ou centré en groupe. Par défaut, le paragraphe mathématique est centré en groupe. Cela signifie que les équations peuvent être alignées les unes par rapport aux autres, mais que l'ensemble du groupe d'équations est centré dans son ensemble. |
| [SetJustification](./setjustification/) | Cela spécifie l'alignement du paragraphe mathématique (une série d'équations adjacentes au sein du même paragraphe). Un paragraphe mathématique peut être aligné à gauche, aligné à droite, centré, ou centré en groupe. Par défaut, le paragraphe mathématique est centré en groupe. Cela signifie que les équations peuvent être alignées les unes par rapport aux autres, mais que l'ensemble du groupe d'équations est centré dans son ensemble. |
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
| [EquationNodeParagraph_CreateNode](./equationnodeparagraph_createnode/) | Créez un nœud du type spécifié. |
