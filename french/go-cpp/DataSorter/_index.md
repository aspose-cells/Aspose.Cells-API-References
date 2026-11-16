---
title: "Classe DataSorter"
linktitle: "DataSorter"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "DataSorter class. Encapsule l'objet qui représente datasorter en Go."
type: docs
weight: 200
url: /fr/go-cpp/datasorter/
---

## DataSorter class

Description résumée pour DataSorter.

```go

type DataSorter struct  {
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
| [GetKeys](./getkeys/) | Obtient la liste des clés du data sorter. |
| [Clear](./clear/) | Effacer tous les paramètres. |
| [GetHasHeaders](./gethasheaders/) | Représente si la plage possède des en-têtes. |
| [SetHasHeaders](./sethasheaders/) | Représente si la plage possède des en-têtes. |
| [AddKey_Int_SortOrder](./addkey_int_sortorder/) | Ajoute l'index de colonne triée et l'ordre de tri. |
| [AddKey_Int_SortOrder_String](./addkey_int_sortorder_string/) | Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée. |
| [AddColorKey](./addcolorkey/) | Ajoute une clé de tri de couleur. |
| [AddKey_Int_SortOnType_SortOrder_Object](./addkey_int_sortontype_sortorder_object/) | Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée. |
| [AddKey_Int_SortOrder_stringArray](./addkey_int_sortorder_stringarray/) | Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée. |
| [GetKey1](./getkey1/) | Représente le premier index de colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [SetKey1](./setkey1/) | Représente le premier index de colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [GetOrder1](./getorder1/) | Représente l'ordre de tri de la première clé. |
| [SetOrder1](./setorder1/) | Représente l'ordre de tri de la première clé. |
| [GetKey2](./getkey2/) | Représente le deuxième index de colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [SetKey2](./setkey2/) | Représente le deuxième index de colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [GetOrder2](./getorder2/) | Représente l'ordre de tri de la deuxième clé. |
| [SetOrder2](./setorder2/) | Représente l'ordre de tri de la deuxième clé. |
| [GetKey3](./getkey3/) | Représente le troisième index de colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [SetKey3](./setkey3/) | Représente le troisième index de colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [GetOrder3](./getorder3/) | Représente l'ordre de tri de la troisième clé. |
| [SetOrder3](./setorder3/) | Représente l'ordre de tri de la troisième clé. |
| [GetSortLeftToRight](./getsortlefttoright/) | True signifie que l'orientation du tri est de gauche à droite.False signifie que l'orientation du tri est de haut en bas.La valeur par défaut est false. |
| [SetSortLeftToRight](./setsortlefttoright/) | True signifie que l'orientation du tri est de gauche à droite.False signifie que l'orientation du tri est de haut en bas.La valeur par défaut est false. |
| [GetCaseSensitive](./getcasesensitive/) | Obtient et définit si la comparaison de chaînes est sensible à la casse. |
| [SetCaseSensitive](./setcasesensitive/) | Obtient et définit si la comparaison de chaînes est sensible à la casse. |
| [GetSortAsNumber](./getsortasnumber/) | Indique si le tri doit traiter tout ce qui ressemble à un nombre. |
| [SetSortAsNumber](./setsortasnumber/) | Indique si le tri doit traiter tout ce qui ressemble à un nombre. |
| [Sort_Cells_Int_Int_Int_Int](./sort_cells_int_int_int_int/) | Trie les données de la zone. |
| [Sort_Cells_CellArea](./sort_cells_cellarea/) | Trie les données de la zone. |
| [Sort](./sort/) | Trie les données de la plage. |
