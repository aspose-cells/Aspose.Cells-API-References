---
title: AutoFilter
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente le filtrage automatique pour la feuille de calcul spécifiée.
type: docs
weight: 90
url: /fr/net/aspose.cells/autofilter/
---
## AutoFilter class

Représente le filtrage automatique pour la feuille de calcul spécifiée.

```csharp
public class AutoFilter
```

## Propriétés

| Nom | La description |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns) { get; } | Obtient la collection des colonnes de filtre. |
| [Range](../../aspose.cells/autofilter/range) { get; set; } | Représente la plage à laquelle s'applique le filtre automatique spécifié. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton) { get; set; } | Indique si le bouton Filtre automatique de cette colonne est visible. |
| [Sorter](../../aspose.cells/autofilter/sorter) { get; } | Obtient le trieur de données. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter)(int, DateTimeGroupingType, int, int, int, int, int, int) | Ajoute un filtre de date. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter)(int, BackgroundType, CellsColor, CellsColor) | Ajoute un filtre de couleur de remplissage. |
| [AddFilter](../../aspose.cells/autofilter/addfilter)(int, string) | Ajoute un filtre pour une colonne de filtre. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter)(int, CellsColor) | Ajoute un filtre de couleur de police. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter)(int, IconSetType, int) | Ajoute un filtre d'icônes. |
| [Custom](../../aspose.cells/autofilter/custom#custom)(int, FilterOperatorType, object) | Filtre une liste avec un critère personnalisé. |
| [Custom](../../aspose.cells/autofilter/custom#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | Filtre une liste avec des critères personnalisés. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter)(int, DynamicFilterType) | Ajoute un filtre dynamique. |
| [Filter](../../aspose.cells/autofilter/filter)(int, string) | Filtre une liste avec des critères spécifiés. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10)(int, bool, bool, int) | Filtrer les 10 premiers éléments de la liste |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea)() | Obtient le[`CellArea`](../cellarea) où le filtre automatique spécifié s'applique à. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks)(int) | Correspond à toutes les cellules vides de la liste. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks)(int) | Correspond à toutes les cellules non vides de la liste. |
| [Refresh](../../aspose.cells/autofilter/refresh#refresh)() | Actualisez les filtres automatiques pour masquer ou afficher les lignes. |
| [Refresh](../../aspose.cells/autofilter/refresh#refresh_1)(bool) | Récupère tous les index des lignes masquées. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter)(int, DateTimeGroupingType, int, int, int, int, int, int) | Supprime un filtre de date. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter#removefilter)(int) | Supprimer le filtre spécifique. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter#removefilter_1)(int, string) | Supprime un filtre pour une colonne de filtre. |
| [SetRange](../../aspose.cells/autofilter/setrange)(int, int, int) | Définit la plage à laquelle s'applique le filtre automatique spécifié. |
| [ShowAll](../../aspose.cells/autofilter/showall)() | Afficher toutes les lignes. |

### Exemples

```csharp

[C#]

//Création d'un flux de fichier contenant le fichier Excel à ouvrir
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook("template.xlsx");
//Accéder à la première feuille de calcul du fichier Excel
Worksheet worksheet = workbook.Worksheets[0];
// Création d'un filtre automatique en donnant la plage de cellules de la ligne d'en-tête
worksheet.AutoFilter.Range = "A1:B1";
//Filtrage des colonnes avec les valeurs spécifiées
worksheet.AutoFilter.Filter(1, "Bananas");
//Enregistrement du fichier Excel modifié.
workbook.Save("output.xls");

[Visual Basic]
   
'Création d'un flux de fichier contenant le fichier Excel à ouvrir
'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook("template.xlsx")
'Accéder à la première feuille de calcul du fichier Excel
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Création d'un filtre automatique en donnant la plage de cellules de la ligne d'en-tête
worksheet.AutoFilter.Range = "A1:B1"
'Filtrage des colonnes avec des valeurs spécifiées
Worksheet.AutoFilter.Filter(1, "Bananas")
'Enregistrement du fichier Excel modifié 
workbook.Save("output.xls")
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
