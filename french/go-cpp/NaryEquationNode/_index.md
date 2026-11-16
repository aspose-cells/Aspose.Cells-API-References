---
title: "Classe NaryEquationNode"
linktitle: "NaryEquationNode"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe NaryEquationNode. Encapsule l'objet qui représente naryequationnode dans Go."
type: docs
weight: 200
url: /fr/go-cpp/naryequationnode/
---

## NaryEquationNode class

Cette classe spécifie une équation d'opérateur n-aire composée d'un opérateur n-aire, d'une base (ou opérande) et de bornes supérieures et inférieures optionnelles.

```go

type NaryEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewNaryEquationNode](./newnaryequationnode/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [IsHideSubscript](./ishidesubscript/) | Afficher la borne inférieure |
| [SetIsHideSubscript](./setishidesubscript/) | Afficher la borne inférieure |
| [IsHideSuperscript](./ishidesuperscript/) | Afficher la borne supérieure |
| [SetIsHideSuperscript](./setishidesuperscript/) | Afficher la borne supérieure |
| [GetLimitLocation](./getlimitlocation/) | Cet attribut spécifie l'emplacement des limites dans les opérateurs n-aires. Les limites peuvent être centrées au-dessus et en dessous de l'opérateur n-aire, ou positionnées juste à droite de l'opérateur. |
| [SetLimitLocation](./setlimitlocation/) | Cet attribut spécifie l'emplacement des limites dans les opérateurs n-aires. Les limites peuvent être centrées au-dessus et en dessous de l'opérateur n-aire, ou positionnées juste à droite de l'opérateur. |
| [GetNaryOperator](./getnaryoperator/) | un opérateur n-aire.e.g "∑".Il est fortement recommandé d'utiliser l'attribut NaryOperatorType pour définir l'opérateur n-aire.Utilisez ce paramètre de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu. |
| [SetNaryOperator](./setnaryoperator/) | un opérateur n-aire.e.g "∑".Il est fortement recommandé d'utiliser l'attribut NaryOperatorType pour définir l'opérateur n-aire.Utilisez ce paramètre de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu. |
| [GetNaryOperatorType](./getnaryoperatortype/) | un opérateur n-aire.e.g "∑" |
| [SetNaryOperatorType](./setnaryoperatortype/) | un opérateur n-aire.e.g "∑" |
| [GetNaryGrow](./getnarygrow/) | Cet attribut spécifie la propriété de croissance des opérateurs n-aires au niveau du document. Lorsqu'il est désactivé, les opérateurs n-aires tels que les intégrales et les sommes ne s'agrandissent pas pour correspondre à la hauteur de leurs opérandes. Lorsqu'il est activé, l'opérateur n-aire s'agrandit verticalement pour correspondre à la hauteur de son opérande. |
| [SetNaryGrow](./setnarygrow/) | Cet attribut spécifie la propriété de croissance des opérateurs n-aires au niveau du document. Lorsqu'il est désactivé, les opérateurs n-aires tels que les intégrales et les sommes ne s'agrandissent pas pour correspondre à la hauteur de leurs opérandes. Lorsqu'il est activé, l'opérateur n-aire s'agrandit verticalement pour correspondre à la hauteur de son opérande. |
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
| [NaryEquationNode_CreateNode](./naryequationnode_createnode/) | Créez un nœud du type spécifié. |
