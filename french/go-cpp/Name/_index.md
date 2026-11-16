---
title: "Classe Name"
linktitle: "Name"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Name. Encapsule l'objet qui représente name en Go."
type: docs
weight: 200
url: /fr/go-cpp/name/
---

## Name class

Représente un nom défini pour une plage de cellules.

```go

type Name struct  {
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
| [GetComment](./getcomment/) | Obtient et définit le commentaire du nom. S'applique uniquement aux versions Excel 2007 ou supérieures. |
| [SetComment](./setcomment/) | Obtient et définit le commentaire du nom. S'applique uniquement aux versions Excel 2007 ou supérieures. |
| [GetText](./gettext/) | Obtient le texte du nom de l'objet. |
| [SetText](./settext/) | Obtient le texte du nom de l'objet. |
| [GetFullText](./getfulltext/) | Obtient le texte complet du nom de l'objet avec le paramètre de portée. |
| [GetRefersTo](./getrefersto/) | Renvoie ou définit la formule à laquelle le nom fait référence, en commençant par un signe égal. |
| [SetRefersTo_String](./setrefersto_string/) | Renvoie ou définit la formule à laquelle le nom fait référence, en commençant par un signe égal. |
| [GetR1C1RefersTo](./getr1c1refersto/) | Obtient ou définit une référence R1C1 du nom. |
| [SetR1C1RefersTo](./setr1c1refersto/) | Obtient ou définit une référence R1C1 du nom. |
| [GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | Obtenez la référence de ce nom. |
| [GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | Obtenez la référence de ce nom en fonction de la cellule spécifiée. |
| [SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | Définissez la référence de ce nom. |
| [IsReferred](./isreferred/) | Indique si ce nom est référencé par d'autres formules. |
| [IsVisible](./isvisible/) | Indique si le nom est visible. |
| [SetIsVisible](./setisvisible/) | Indique si le nom est visible. |
| [GetSheetIndex](./getsheetindex/) | Indique si ce nom appartient à un classeur ou à une feuille de calcul. 0 = nom global, sinon indice de la feuille (à partir de 1). |
| [SetSheetIndex](./setsheetindex/) | Indique si ce nom appartient à un classeur ou à une feuille de calcul. 0 = nom global, sinon indice de la feuille (à partir de 1). |
| [ToString](./tostring/) | Renvoie une chaîne qui représente l'objet Range actuel. |
| [GetRanges](./getranges/) | Obtient toutes les plages référencées par ce nom. |
| [GetRanges_Bool](./getranges_bool/) | Obtient toutes les plages référencées par ce nom. |
| [GetReferredAreas](./getreferredareas/) | Obtient toutes les références référencées par ce nom. |
| [GetRange](./getrange/) | Obtient la plage si ce nom fait référence à une plage. |
| [GetRange_Bool](./getrange_bool/) | Obtient la plage si ce nom fait référence à une plage |
| [GetRange_Int_Int_Int](./getrange_int_int_int/) | Obtient la plage si ce nom fait référence à une plage. Si la référence de ce nom n’est pas absolue, la plage peut varier selon la cellule. |
