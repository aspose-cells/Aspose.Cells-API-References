---
title: Protection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente les différents types doptions de protection disponibles pour une feuille de calcul.
type: docs
weight: 4910
url: /fr/net/aspose.cells/protection/
---
## Protection class

Représente les différents types d'options de protection disponibles pour une feuille de calcul.

```csharp
public class Protection
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn) { get; set; } | Représente si la suppression de colonnes est autorisée sur une feuille de calcul protégée. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow) { get; set; } | Représente si la suppression de lignes est autorisée sur une feuille de calcul protégée. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent) { get; set; } | Représente si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille de calcul protégée. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject) { get; set; } | Représente si l'utilisateur est autorisé à manipuler des objets de dessin sur une feuille de calcul protégée. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario) { get; set; } | Représente si l'utilisateur est autorisé à modifier des scénarios sur une feuille de calcul protégée. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering) { get; set; } | Représente si l'utilisateur est autorisé à utiliser un filtre automatique créé avant que la feuille ne soit protégée. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell) { get; set; } | Indique si la mise en forme des cellules est autorisée sur une feuille de calcul protégée. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn) { get; set; } | Représente si le formatage des colonnes est autorisé sur une feuille de calcul protégée |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow) { get; set; } | Représente si le formatage des lignes est autorisé sur une feuille de calcul protégée |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn) { get; set; } | Représente si l'insertion de colonnes est autorisée sur une feuille de calcul protégée |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink) { get; set; } | Représente si l'insertion de liens hypertexte est autorisée sur une feuille de calcul protégée |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow) { get; set; } | Représente si l'insertion de lignes est autorisée sur une feuille de calcul protégée |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell) { get; set; } | Indique si l'utilisateur est autorisé à sélectionner des cellules verrouillées dans une feuille de calcul protégée. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell) { get; set; } | Représente si l'utilisateur est autorisé à sélectionner des cellules déverrouillées sur une feuille de calcul protégée. |
| [AllowSorting](../../aspose.cells/protection/allowsorting) { get; set; } | Représente si l'option de tri est autorisée sur une feuille de calcul protégée. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable) { get; set; } | Représente si l'utilisateur est autorisé à manipuler des tableaux croisés dynamiques sur une feuille de calcul protégée. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword) { get; } | Indique si les feuilles de calcul sont protégées par mot de passe. |
| [Password](../../aspose.cells/protection/password) { get; set; } | Représente le mot de passe pour protéger la feuille de calcul. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy)(Protection) | Informations sur la protection contre la copie. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash)() | Obtient le hachage du mot de passe actuel. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword)(string) | Vérifie le mot de passe. |

### Exemples

```csharp

[C#]
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();

Worksheet worksheet = workbook.Worksheets[0];
// Autoriser les utilisateurs à sélectionner des cellules verrouillées de la feuille de calcul
worksheet.Protection.AllowSelectingLockedCell = true;
// Autoriser les utilisateurs à sélectionner des cellules déverrouillées de la feuille de calcul
worksheet.Protection.AllowSelectingUnlockedCell = true;  

[Visual Basic]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Permettre aux utilisateurs de sélectionner des cellules verrouillées de la feuille de calcul
worksheet.Protection.AllowSelectingLockedCell = True
'Permettre aux utilisateurs de sélectionner des cellules déverrouillées de la feuille de calcul
worksheet.Protection.AllowSelectingUnlockedCell = True
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
