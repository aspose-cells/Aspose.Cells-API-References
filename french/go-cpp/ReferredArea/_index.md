---
title: "Classe ReferredArea"
linktitle: "ReferredArea"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe ReferredArea. Encapsule l'objet qui représente referredarea en Go."
type: docs
weight: 200
url: /fr/go-cpp/referredarea/
---

## ReferredArea class

Représente une zone référencée par la formule.

```go

type ReferredArea struct  {
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
| [IsExternalLink](./isexternallink/) | Indique si c'est un lien externe. |
| [GetExternalFileName](./getexternalfilename/) | Obtient le nom du fichier externe si c'est une référence externe. |
| [GetSheetName](./getsheetname/) | Indique dans quelle feuille cette référence se trouve. |
| [GetSheetNames](./getsheetnames/) | Noms de toutes les feuilles de calcul auxquelles cette instance fait référence. |
| [IsEntireRow](./isentirerow/) | Indique si cette zone contient toutes les colonnes (ligne entière). |
| [IsEntireColumn](./isentirecolumn/) | Indique si cette zone contient toutes les lignes (colonne entière). |
| [IsArea](./isarea/) | Indique si c'est une zone. |
| [GetEndColumn](./getendcolumn/) | La colonne de fin de la zone. |
| [GetStartColumn](./getstartcolumn/) | La colonne de départ de la zone. |
| [GetEndRow](./getendrow/) | La ligne de fin de la zone. |
| [GetStartRow](./getstartrow/) | La ligne de départ de la zone. |
| [GetValues](./getvalues/) | Obtient les valeurs des cellules dans cette zone. |
| [GetValues_Bool](./getvalues_bool/) | Obtient les valeurs des cellules dans cette zone. |
| [GetValue_Int_Int](./getvalue_int_int/) | Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone. |
| [GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone. |
| [ToString](./tostring/) | Renvoie l'adresse de référence de cette zone. Généralement, il s'agit de l'adresse de la référence qui peut être utilisée dans une formule, telle que "Sheet1!A1:C3". |
