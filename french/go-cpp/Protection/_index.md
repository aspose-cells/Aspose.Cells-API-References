---
title: "Protection Classe"
linktitle: "Protection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Protection classe. Encapsule l'objet qui représente protection en Go."
type: docs
weight: 200
url: /fr/go-cpp/protection/
---

## Protection class

Représente les différents types d'options de protection disponibles pour une feuille de calcul.

```go

type Protection struct  {
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
| [Copy](./copy/) | Copier les informations de protection. |
| [GetAllowDeletingColumn](./getallowdeletingcolumn/) | Représente si la suppression des colonnes est autorisée sur une feuille de calcul protégée. |
| [SetAllowDeletingColumn](./setallowdeletingcolumn/) | Représente si la suppression des colonnes est autorisée sur une feuille de calcul protégée. |
| [GetAllowDeletingRow](./getallowdeletingrow/) | Représente si la suppression des lignes est autorisée sur une feuille de calcul protégée. |
| [SetAllowDeletingRow](./setallowdeletingrow/) | Représente si la suppression des lignes est autorisée sur une feuille de calcul protégée. |
| [GetAllowFiltering](./getallowfiltering/) | Représente si l'utilisateur est autorisé à utiliser un AutoFilter qui a été créé avant que la feuille ne soit protégée. |
| [SetAllowFiltering](./setallowfiltering/) | Représente si l'utilisateur est autorisé à utiliser un AutoFilter qui a été créé avant que la feuille ne soit protégée. |
| [GetAllowFormattingCell](./getallowformattingcell/) | Représente si le formatage des cellules est autorisé sur une feuille de calcul protégée. |
| [SetAllowFormattingCell](./setallowformattingcell/) | Représente si le formatage des cellules est autorisé sur une feuille de calcul protégée. |
| [GetAllowFormattingColumn](./getallowformattingcolumn/) | Représente si le formatage des colonnes est autorisé sur une feuille de calcul protégée |
| [SetAllowFormattingColumn](./setallowformattingcolumn/) | Représente si le formatage des colonnes est autorisé sur une feuille de calcul protégée |
| [GetAllowFormattingRow](./getallowformattingrow/) | Représente si le formatage des lignes est autorisé sur une feuille de calcul protégée |
| [SetAllowFormattingRow](./setallowformattingrow/) | Représente si le formatage des lignes est autorisé sur une feuille de calcul protégée |
| [GetAllowInsertingColumn](./getallowinsertingcolumn/) | Représente si l'insertion des colonnes est autorisée sur une feuille de calcul protégée |
| [SetAllowInsertingColumn](./setallowinsertingcolumn/) | Représente si l'insertion des colonnes est autorisée sur une feuille de calcul protégée |
| [GetAllowInsertingHyperlink](./getallowinsertinghyperlink/) | Représente si l'insertion des hyperliens est autorisée sur une feuille de calcul protégée |
| [SetAllowInsertingHyperlink](./setallowinsertinghyperlink/) | Représente si l'insertion des hyperliens est autorisée sur une feuille de calcul protégée |
| [GetAllowInsertingRow](./getallowinsertingrow/) | Représente si l'insertion des lignes est autorisée sur une feuille de calcul protégée |
| [SetAllowInsertingRow](./setallowinsertingrow/) | Représente si l'insertion des lignes est autorisée sur une feuille de calcul protégée |
| [GetAllowSorting](./getallowsorting/) | Représente si l'option de tri est autorisée sur une feuille de calcul protégée. |
| [SetAllowSorting](./setallowsorting/) | Représente si l'option de tri est autorisée sur une feuille de calcul protégée. |
| [GetAllowUsingPivotTable](./getallowusingpivottable/) | Représente si l'utilisateur est autorisé à manipuler les tableaux croisés dynamiques sur une feuille de calcul protégée. |
| [SetAllowUsingPivotTable](./setallowusingpivottable/) | Représente si l'utilisateur est autorisé à manipuler les tableaux croisés dynamiques sur une feuille de calcul protégée. |
| [GetAllowEditingContent](./getalloweditingcontent/) | Représente si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille de calcul protégée. |
| [SetAllowEditingContent](./setalloweditingcontent/) | Représente si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille de calcul protégée. |
| [GetAllowEditingObject](./getalloweditingobject/) | Représente si l'utilisateur est autorisé à manipuler les objets de dessin sur une feuille de calcul protégée. |
| [SetAllowEditingObject](./setalloweditingobject/) | Représente si l'utilisateur est autorisé à manipuler les objets de dessin sur une feuille de calcul protégée. |
| [GetAllowEditingScenario](./getalloweditingscenario/) | Représente si l'utilisateur est autorisé à modifier les scénarios sur une feuille de calcul protégée. |
| [SetAllowEditingScenario](./setalloweditingscenario/) | Représente si l'utilisateur est autorisé à modifier les scénarios sur une feuille de calcul protégée. |
| [GetAllowSelectingLockedCell](./getallowselectinglockedcell/) | Représente si l'utilisateur est autorisé à sélectionner les cellules verrouillées sur une feuille de calcul protégée. |
| [SetAllowSelectingLockedCell](./setallowselectinglockedcell/) | Représente si l'utilisateur est autorisé à sélectionner les cellules verrouillées sur une feuille de calcul protégée. |
| [GetAllowSelectingUnlockedCell](./getallowselectingunlockedcell/) | Représente si l'utilisateur est autorisé à sélectionner les cellules déverrouillées sur une feuille de calcul protégée. |
| [SetAllowSelectingUnlockedCell](./setallowselectingunlockedcell/) | Représente si l'utilisateur est autorisé à sélectionner les cellules déverrouillées sur une feuille de calcul protégée. |
| [GetPassword](./getpassword/) | Représente le mot de passe pour protéger la feuille de calcul. |
| [SetPassword](./setpassword/) | Représente le mot de passe pour protéger la feuille de calcul. |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Indique si les feuilles de calcul sont protégées par un mot de passe. |
| [VerifyPassword](./verifypassword/) | Vérifie le mot de passe. |
| [GetPasswordHash](./getpasswordhash/) | Obtient le hachage du mot de passe actuel. |
