---
title: "Classe Row"
linktitle: "Row"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Row. Encapsule l'objet qui représente une ligne en Go."
type: docs
weight: 200
url: /fr/go-cpp/row/
---

## Row class

Représente une seule ligne dans une feuille de calcul.

```go

type Row struct  {
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
| [GetCellByIndex](./getcellbyindex/) | Obtenez la cellule par indice spécifique dans la collection de cellules de cette ligne. |
| [IsBlank](./isblank/) | Indique si la ligne contient des données |
| [Get](./get/) | Obtient la cellule. |
| [GetEnumerator](./getenumerator/) | Obtient l'énumérateur des cellules |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Obtient un énumérateur qui parcourt les cellules de cette ligne. |
| [GetCellOrNull](./getcellornull/) | Obtient la cellule ou null à l'indice spécifique. |
| [IsCollapsed](./iscollapsed/) | si la ligne est réduite |
| [SetIsCollapsed](./setiscollapsed/) | si la ligne est réduite |
| [GetHeight](./getheight/) | Obtient et définit la hauteur de la ligne en points. |
| [SetHeight](./setheight/) | Obtient et définit la hauteur de la ligne en points. |
| [IsHidden](./ishidden/) | Indique si la ligne est masquée. |
| [SetIsHidden](./setishidden/) | Indique si la ligne est masquée. |
| [GetIndex](./getindex/) | Obtient l'index de cette ligne. |
| [GetGroupLevel](./getgrouplevel/) | Obtient le niveau de groupe de la ligne. |
| [SetGroupLevel](./setgrouplevel/) | Obtient le niveau de groupe de la ligne. |
| [IsHeightMatched](./isheightmatched/) | Indique si la hauteur de la ligne correspond au paramètre de police par défaut actuel du classeur. Vrai pour cette propriété indique également que la hauteur de la ligne est \"automatique\" sans valeur de hauteur personnalisée définie par l'utilisateur. |
| [SetIsHeightMatched](./setisheightmatched/) | Indique si la hauteur de la ligne correspond au paramètre de police par défaut actuel du classeur. Vrai pour cette propriété indique également que la hauteur de la ligne est \"automatique\" sans valeur de hauteur personnalisée définie par l'utilisateur. |
| [GetStyle](./getstyle/) | Obtient le style de cette ligne. |
| [SetStyle](./setstyle/) | Définit le style de cette ligne. |
| [GetHasCustomStyle](./gethascustomstyle/) | Indique si cette ligne possède des paramètres de style personnalisés (différents de ceux par défaut hérités du classeur). |
| [CopySettings](./copysettings/) | Copie les paramètres de la ligne, tels que le style, la hauteur, la visibilité, ...etc. |
| [GetFirstCell](./getfirstcell/) | Obtient le premier objet cellule dans la ligne. |
| [GetFirstDataCell](./getfirstdatacell/) | Obtient la première cellule non vide dans la ligne. |
| [GetLastCell](./getlastcell/) | Obtient le dernier objet cellule dans la ligne. |
| [GetLastDataCell](./getlastdatacell/) | Obtient la dernière cellule non vide dans la ligne. |
| [ApplyStyle](./applystyle/) | Applique les formats à une ligne entière. |
| [Equals_Object](./equals_object/) | Vérifie si cet objet fait référence à la même ligne qu'un autre. |
| [Equals_Row](./equals_row/) | Vérifie si cet objet fait référence à la même ligne qu'un autre objet ligne. |
