---
title: "Classe UnionRange"
linktitle: "UnionRange"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe UnionRange. Encapsule l'objet qui représente unionrange en Go."
type: docs
weight: 200
url: /fr/go-cpp/unionrange/
---

## UnionRange class

Représente la plage d'union.

```go

type UnionRange struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetFirstRow](./getfirstrow/) | Obtient l'index de la première ligne de la plage. |
| [GetFirstColumn](./getfirstcolumn/) | Obtient l'index de la première colonne de la plage. |
| [GetRowCount](./getrowcount/) | Obtient le nombre de lignes dans la plage. |
| [GetColumnCount](./getcolumncount/) | Obtient le nombre de lignes dans la plage. |
| [Merge](./merge/) | Combine une plage de cellules en une seule cellule. |
| [UnMerge](./unmerge/) | Démarque les cellules fusionnées de cette plage. |
| [PutValue](./putvalue/) | Place une valeur dans la plage, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [GetValue](./getvalue/) | Obtient et définit les valeurs de la plage. |
| [SetValue](./setvalue/) | Obtient et définit les valeurs de la plage. |
| [GetName](./getname/) | Obtient ou définit le nom de la plage. |
| [SetName](./setname/) | Obtient ou définit le nom de la plage. |
| [GetRefersTo](./getrefersto/) | Obtient la référence de la plage. |
| [GetHasRange](./gethasrange/) | Indique si cela possède une plage. |
| [GetHyperlinks](./gethyperlinks/) | Obtient tous les hyperliens dans la plage. |
| [SetStyle](./setstyle/) | Définit le style de la plage. |
| [ApplyStyle](./applystyle/) | Applique des formats à l'ensemble d'une plage. |
| [Copy](./copy/) | Copie la plage avec les options de collage spécial. |
| [GetEnumerator](./getenumerator/) | Obtient l'énumérateur des cellules de cette Range. |
| [GetCellCount](./getcellcount/) | Obtient le nombre total de cellules dans la plage. |
| [GetRangeCount](./getrangecount/) | Obtient le nombre de plages. |
| [GetRanges](./getranges/) | Obtient toutes les plages d'union. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Définit les bordures de contour autour d'une plage de cellules. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Définit les bordures de contour autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [Intersect_String](./intersect_string/) | Intersecte une autre plage. |
| [Intersect_UnionRange](./intersect_unionrange/) | Intersecte une autre plage. |
| [Intersect_RangeArray](./intersect_rangearray/) | Intersecte une autre plage. |
| [Union_String](./union_string/) | Fusionner une autre plage. |
| [Union_UnionRange](./union_unionrange/) | Fusionner une autre plage. |
| [Union_RangeArray](./union_rangearray/) | Fusionner les plages. |
