---
title: "Classe DelimiterEquationNode"
linktitle: "DelimiterEquationNode"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe DelimiterEquationNode. Encapsule l'objet qui représente delimiterequationnode en Go."
type: docs
weight: 200
url: /fr/go-cpp/delimiterequationnode/
---

## DelimiterEquationNode class

Cette classe spécifie l'équation de délimiteur, composée de délimiteurs ouvrants et fermants (tels que les parenthèses, accolades, crochets et barres verticales), et d'un composant contenu à l'intérieur. Le délimiteur peut contenir plusieurs composants, avec un caractère séparateur désigné entre chaque composant.

```go

type DelimiterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewDelimiterEquationNode](./newdelimiterequationnode/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetBeginChar](./getbeginchar/) | Caractère de début du délimiteur. |
| [SetBeginChar](./setbeginchar/) | Caractère de début du délimiteur. |
| [GetEndChar](./getendchar/) | Caractère de fin du délimiteur. |
| [SetEndChar](./setendchar/) | Caractère de fin du délimiteur. |
| [GetNaryGrow](./getnarygrow/) | Spécifie si le délimiteur doit s'étendre et se contracter automatiquement avec la hauteur de la formule. |
| [SetNaryGrow](./setnarygrow/) | Spécifie si le délimiteur doit s'étendre et se contracter automatiquement avec la hauteur de la formule. |
| [GetSeparatorChar](./getseparatorchar/) | Caractère séparateur du délimiteur. |
| [SetSeparatorChar](./setseparatorchar/) | Caractère séparateur du délimiteur. |
| [GetDelimiterShape](./getdelimitershape/) | Spécifie la forme des délimiteurs dans l'objet délimiteur. |
| [SetDelimiterShape](./setdelimitershape/) | Spécifie la forme des délimiteurs dans l'objet délimiteur. |
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
| [DelimiterEquationNode_CreateNode](./delimiterequationnode_createnode/) | Créez un nœud du type spécifié. |
