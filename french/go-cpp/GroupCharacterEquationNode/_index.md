---
title: "Classe GroupCharacterEquationNode"
linktitle: "GroupCharacterEquationNode"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe GroupCharacterEquationNode. Encapsule l'objet qui représente groupcharacterequationnode en Go."
type: docs
weight: 200
url: /fr/go-cpp/groupcharacterequationnode/
---

## GroupCharacterEquationNode class

Cette classe spécifie la fonction Groupe-Caractère, consistant en un caractère placé au-dessus ou au-dessous du texte, souvent dans le but de regrouper visuellement des éléments.

```go

type GroupCharacterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewGroupCharacterEquationNode](./newgroupcharacterequationnode/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetGroupChr](./getgroupchr/) | Spécifie un symbole (par défaut U+23DF). Il est fortement recommandé d'utiliser l'attribut ChrType pour définir le caractère d'accent. Utilisez ce réglage de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu. |
| [SetGroupChr](./setgroupchr/) | Spécifie un symbole (par défaut U+23DF). Il est fortement recommandé d'utiliser l'attribut ChrType pour définir le caractère d'accent. Utilisez ce réglage de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu. |
| [GetChrType](./getchrtype/) | Spécifiez les caractères combinés par valeur de type. |
| [SetChrType](./setchrtype/) | Spécifiez les caractères combinés par valeur de type. |
| [GetPosition](./getposition/) | Cet attribut spécifie la position du caractère dans l'objet |
| [SetPosition](./setposition/) | Cet attribut spécifie la position du caractère dans l'objet |
| [GetVertJc](./getvertjc/) | Cet attribut, combiné avec pos de groupChrPr, spécifie la disposition verticale de l'objet groupChr. Où pos indique la position du caractère de regroupement, vertJc indique l'alignement de l'objet par rapport à la ligne de base. |
| [SetVertJc](./setvertjc/) | Cet attribut, combiné avec pos de groupChrPr, spécifie la disposition verticale de l'objet groupChr. Où pos indique la position du caractère de regroupement, vertJc indique l'alignement de l'objet par rapport à la ligne de base. |
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
| [GroupCharacterEquationNode_CreateNode](./groupcharacterequationnode_createnode/) | Créez un nœud du type spécifié. |
