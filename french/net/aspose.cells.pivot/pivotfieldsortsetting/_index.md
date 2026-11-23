---
title: "Class PivotFieldSortSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Pivot.PivotFieldSortSetting class. Représente le paramètre de tri des champs de tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

Représente le paramètre de tri des champs de tableau croisé dynamique.

```csharp
public class PivotFieldSortSetting
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | Trie selon les valeurs dans la ligne ou la colonne. |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; set; } | (**Obsolete.**) Représente l'index du champ trié par. -1 signifie trier le PivotField par les libellés, les autres signifient trier par le champ de données. |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; set; } | Indique si une opération de tri de données simple sera appliquée. |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | Indique s'il faut trier le champ lui-même ou le champ de données. |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | Le type de ligne pivot trié par. |
| [SortBy](../../aspose.cells.pivot/pivotfieldsortsetting/sortby/) { get; set; } | Représente l'index du champ trié par. Une valeur de -1 indique un tri par les propres valeurs de l'élément pivot. Lorsqu'elle est supérieure ou égale à zéro, elle représente l'index du champ de données dans la région de données. |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; set; } | Représente le [`SortOrder`](../../aspose.cells/sortorder/). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtenez le paramètre de tri du champ pivot à partir du tableau croisé dynamique
            // Remarque : cela suppose que le tableau croisé dynamique possède des paramètres de tri accessibles
            // Puisque nous ne pouvons pas créer directement un nouveau PivotFieldSortSetting
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // Propriétés d'affichage (lecture seule)
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // Appliquer le tri au tableau croisé dynamique (le tri réel serait effectué via les méthodes du tableau croisé dynamique)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrer le résultat
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


