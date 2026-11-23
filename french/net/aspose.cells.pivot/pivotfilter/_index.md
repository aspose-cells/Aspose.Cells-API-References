---
title: "Classe PivotFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Pivot.PivotFilter class. Représente un PivotFilter dans la collection PivotFilter"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

Représente un **PivotFilter** dans la collection **PivotFilter**.

```csharp
public class PivotFilter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter/) { get; } | (**Obsolete.**) Obtient l'autofiltre du filtre pivot. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder/) { get; set; } | Obtient l'ordre d'évaluation du filtre pivot. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex/) { get; } | Obtient l'index du champ source auquel ce filtre pivot est appliqué. |
| [FilterCategory](../../aspose.cells.pivot/pivotfilter/filtercategory/) { get; } | Obtient la catégorie de ce filtre. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype/) { get; } | Obtient le type de filtre du filtre pivot. |
| [MeasureCubeFieldIndex](../../aspose.cells.pivot/pivotfilter/measurecubefieldindex/) { get; } | Spécifie l'index du champ cube de mesure. Cette propriété n'est utilisée que par les filtres dans les tableaux croisés dynamiques OLAP et indique sur quelle mesure un filtre de valeur doit s'appliquer. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex/) { get; set; } | (**Obsolete.**) Obtient l'index du champ de mesure du filtre pivot. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/) { get; set; } | Obtient l'index du champ de propriété du membre du filtre pivot. |
| [Name](../../aspose.cells.pivot/pivotfilter/name/) { get; set; } | Obtient le nom du filtre pivot. |
| [UseWholeDay](../../aspose.cells.pivot/pivotfilter/usewholeday/) { get; set; } | Indique s'il faut utiliser des jours complets dans ses critères de filtrage de dates. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1/) { get; set; } | Obtient la chaîne value1 du filtre pivot d'étiquette. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2/) { get; set; } | Obtient la chaîne value2 du filtre pivot d'étiquette. |
| [ValueFieldIndex](../../aspose.cells.pivot/pivotfilter/valuefieldindex/) { get; set; } | Obtient l'index du champ de valeur dans la région de valeur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetDateTimeValues](../../aspose.cells.pivot/pivotfilter/getdatetimevalues/)() | Obtient les valeurs du filtre numérique. |
| [GetLabels](../../aspose.cells.pivot/pivotfilter/getlabels/)() | Obtient les libellés du filtre de légende. |
| [GetNumberValues](../../aspose.cells.pivot/pivotfilter/getnumbervalues/)() | Obtient les valeurs du filtre numérique. |
| [GetTop10Value](../../aspose.cells.pivot/pivotfilter/gettop10value/)() | Obtient le paramètre top 10 du filtre. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterDemo
    {
        public static void PivotFilterExample()
        {
            // Créer un nouveau classeur
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Remplit la feuille de calcul avec des données d'exemple
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Définissez le style du tableau croisé dynamique
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Ajouter un filtre pivot
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Définir des propriétés supplémentaires pour le filtre pivot
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // Actualiser et calculer les données du tableau croisé dynamique
            pivot.RefreshData();
            pivot.CalculateData();

            // Enregistrez le classeur
            book.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


