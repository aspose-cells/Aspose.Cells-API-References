---
title: "Classe AutoFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.AutoFilter. Représente le filtrage automatique pour la feuille de calcul spécifiée"
type: docs
url: /fr/net/aspose.cells/autofilter/
---
## AutoFilter class

Représente le filtrage automatique pour la feuille de calcul spécifiée.

```csharp
public class AutoFilter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns/) { get; } | Obtient la collection des colonnes de filtre. |
| [Range](../../aspose.cells/autofilter/range/) { get; set; } | Représente la plage à laquelle le AutoFilter spécifié s'applique. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton/) { get; set; } | Indique si le bouton AutoFilter pour cette colonne est visible. |
| [Sorter](../../aspose.cells/autofilter/sorter/) { get; } | Obtient le trieur de données. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Ajoute un filtre de date. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter/)(int, BackgroundType, CellsColor, CellsColor) | Ajoute un filtre de couleur de remplissage. |
| [AddFilter](../../aspose.cells/autofilter/addfilter/)(int, string) | Ajoute un filtre pour une colonne de filtre. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter/)(int, CellsColor) | Ajoute un filtre de couleur de police. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter/)(int, IconSetType, int) | Ajoute un filtre d'icône. |
| [Custom](../../aspose.cells/autofilter/custom/#custom)(int, FilterOperatorType, object) | Filtre une liste avec un critère personnalisé. |
| [Custom](../../aspose.cells/autofilter/custom/#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | Filtre une liste avec des critères personnalisés. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter/)(int, DynamicFilterType) | Ajoute un filtre dynamique. |
| [Filter](../../aspose.cells/autofilter/filter/)(int, string) | Filtre une liste avec des critères spécifiés. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10/)(int, bool, bool, int) | Filtrer les 10 meilleurs éléments de la liste |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea)() | Obtient le [`CellArea`](../cellarea/) où ce AutoFilter s'applique. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea_1)(bool) | Obtient le [`CellArea`](../cellarea/) où le AutoFilter spécifié s'applique. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks/)(int) | Correspond à toutes les cellules vides de la liste. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks/)(int) | Correspond à toutes les cellules non vides de la liste. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh)() | Actualise les filtres automatiques pour masquer ou afficher les lignes. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh_1)(bool) | Obtient tous les index des lignes masquées. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Supprime un filtre de date. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter)(int) | Supprime le filtre spécifique. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter_1)(int, string) | Supprime un filtre pour une colonne de filtre. |
| [SetRange](../../aspose.cells/autofilter/setrange/)(int, int, int) | Définit la plage à laquelle le AutoFilter spécifié s'applique. |
| [ShowAll](../../aspose.cells/autofilter/showall/)() | Afficher toutes les lignes. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterDemo
    {
        public static void AutoFilterExample()
        {
            // Création d'un flux de fichier contenant le fichier Excel à ouvrir
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accéder à la première feuille de calcul du fichier Excel
            Worksheet worksheet = workbook.Worksheets[0];
            // Création d'un AutoFilter en fournissant la plage de cellules de la ligne d'en-tête
            worksheet.AutoFilter.Range = "A1:B8";
            // Filtrage des colonnes avec des valeurs spécifiées
            worksheet.AutoFilter.Filter(0, "Bananas");
            worksheet.AutoFilter.Refresh();

            // Enregistrement du fichier Excel modifié.
            workbook.Save("AutoFilterExample.xlsx");
            workbook.Save("AutoFilterExample.pdf");

            // Instanciation d'un objet Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accéder à la première feuille de calcul du fichier Excel
            worksheet = workbook.Worksheets[0];

            // Code supplémentaire pour démontrer d'autres fonctionnalités de l'AutoFilter
            // Définition de la plage pour l'AutoFilter
            worksheet.AutoFilter.Range = "A1:B8";
            // Ajout d'un filtre
            worksheet.AutoFilter.AddFilter(0, "Apples");
            // Ajout d'un filtre de date
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // Enregistrement du fichier Excel modifié.
            workbook.Save("AutoFilterExample2.xlsx");
            workbook.Save("AutoFilterExample2.pdf");

            // Instanciation d'un objet Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accéder à la première feuille de calcul du fichier Excel
            worksheet = workbook.Worksheets[0];
                        
            // Ajout d'un filtre de couleur de police
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // Enregistrement du fichier Excel modifié.
            workbook.Save("AutoFilterExample3.xlsx");
            workbook.Save("AutoFilterExample3.pdf");

            // Instanciation d'un objet Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accéder à la première feuille de calcul du fichier Excel
            worksheet = workbook.Worksheets[0];

            // Ajout d'un filtre de couleur de remplissage
            CellsColor foregroundColor = workbook.CreateCellsColor();
            foregroundColor.Color = System.Drawing.Color.Red;
            CellsColor backgroundColor = workbook.CreateCellsColor();
            backgroundColor.Color = System.Drawing.Color.White;

            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, foregroundColor, backgroundColor);

            worksheet.AutoFilter.Refresh();
            // Enregistrement du fichier Excel modifié.
            workbook.Save("AutoFilterExample4.xlsx");
            workbook.Save("AutoFilterExample4.pdf");

            // Instanciation d'un objet Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accéder à la première feuille de calcul du fichier Excel
            worksheet = workbook.Worksheets[0];

            // Correspondance aux cellules vides
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Enregistrement du fichier Excel modifié.
            workbook.Save("AutoFilterExample5.xlsx");
            workbook.Save("AutoFilterExample5.pdf");

            // Instanciation d'un objet Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accéder à la première feuille de calcul du fichier Excel
            worksheet = workbook.Worksheets[0];

            // Correspondance aux cellules non vides
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Enregistrement du fichier Excel modifié.
            workbook.Save("AutoFilterExample6.xlsx");
            workbook.Save("AutoFilterExample6.pdf");

            // Instanciation d'un objet Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accéder à la première feuille de calcul du fichier Excel
            worksheet = workbook.Worksheets[0];

            // Filtre personnalisé
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "Test");

            worksheet.AutoFilter.Refresh();
            // Enregistrement du fichier Excel modifié.
            workbook.Save("AutoFilterExample7.xlsx");
            workbook.Save("AutoFilterExample7.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


