---
title: "Classe Protection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Protection. Représente les différents types d'options de protection disponibles pour une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/protection/
---
## Protection class

Représente les différents types d'options de protection disponibles pour une feuille de calcul.

```csharp
public class Protection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn/) { get; set; } | Représente si la suppression de colonnes est autorisée sur une feuille de calcul protégée. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow/) { get; set; } | Représente si la suppression de lignes est autorisée sur une feuille de calcul protégée. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent/) { get; set; } | Représente si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille de calcul protégée. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject/) { get; set; } | Représente si l'utilisateur est autorisé à manipuler les objets de dessin sur une feuille de calcul protégée. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario/) { get; set; } | Représente si l'utilisateur est autorisé à modifier les scénarios sur une feuille de calcul protégée. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering/) { get; set; } | Représente si l'utilisateur est autorisé à utiliser un AutoFilter créé avant que la feuille ne soit protégée. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell/) { get; set; } | Représente si le formatage des cellules est autorisé sur une feuille de calcul protégée. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn/) { get; set; } | Représente si le formatage des colonnes est autorisé sur une feuille de calcul protégée |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow/) { get; set; } | Représente si le formatage des lignes est autorisé sur une feuille de calcul protégée |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn/) { get; set; } | Représente si l'insertion de colonnes est autorisée sur une feuille de calcul protégée |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink/) { get; set; } | Représente si l'insertion d'hyperliens est autorisée sur une feuille de calcul protégée |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow/) { get; set; } | Représente si l'insertion de lignes est autorisée sur une feuille de calcul protégée |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell/) { get; set; } | Représente si l'utilisateur est autorisé à sélectionner les cellules verrouillées sur une feuille de calcul protégée. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell/) { get; set; } | Représente si l'utilisateur est autorisé à sélectionner les cellules déverrouillées sur une feuille de calcul protégée. |
| [AllowSorting](../../aspose.cells/protection/allowsorting/) { get; set; } | Représente si l'option de tri est autorisée sur une feuille de calcul protégée. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable/) { get; set; } | Représente si l'utilisateur est autorisé à manipuler les tableaux croisés dynamiques sur une feuille de calcul protégée. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword/) { get; } | Indique si la feuille de calcul est protégée par un mot de passe. |
| [Password](../../aspose.cells/protection/password/) { get; set; } | Représente le mot de passe pour protéger la feuille de calcul. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy/)(Protection) | Copier les informations de protection. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash/)() | Obtient le hachage du mot de passe actuel. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword/)(string) | Vérifie le mot de passe. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionDemo
    {
        public static void ProtectionExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder aux paramètres de protection de la feuille de calcul
            Protection protection = worksheet.Protection;

            // Définir diverses propriétés de protection
            protection.AllowDeletingColumn = true;
            protection.AllowDeletingRow = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingCell = true;
            protection.AllowFormattingColumn = true;
            protection.AllowFormattingRow = true;
            protection.AllowInsertingColumn = true;
            protection.AllowInsertingHyperlink = true;
            protection.AllowInsertingRow = true;
            protection.AllowSorting = true;
            protection.AllowUsingPivotTable = true;
            protection.AllowEditingContent = true;
            protection.AllowEditingObject = true;
            protection.AllowEditingScenario = true;
            protection.Password = "password123";
            protection.AllowSelectingLockedCell = true;
            protection.AllowSelectingUnlockedCell = true;

            // Vérifier si la feuille de calcul est protégée par un mot de passe
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;

            // Enregistrement du classeur
            workbook.Save("ProtectionExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


