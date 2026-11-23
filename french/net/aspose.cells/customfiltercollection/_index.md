---
title: "Classe CustomFilterCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CustomFilterCollection. Représente les filtres personnalisés"
type: docs
url: /fr/net/aspose.cells/customfiltercollection/
---
## CustomFilterCollection class

Représente les filtres personnalisés.

```csharp
public class CustomFilterCollection : CollectionBase<CustomFilter>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CustomFilterCollection](customfiltercollection/)() | (**Obsolete.**) Construit une nouvelle instance. |

## Propriétés

| Nom | Description |
| --- | --- |
| [And](../../aspose.cells/customfiltercollection/and/) { get; set; } | Indique si les deux critères ont une relation "et". |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/customfiltercollection/item/) { get; } | Obtient le filtre personnalisé à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomFilter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomFilter, IComparer&lt;CustomFilter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomFilter, IComparer&lt;CustomFilter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomFilter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomFilter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomFilter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomFilter[], int, int) |  |
| [Custom](../../aspose.cells/customfiltercollection/custom/)(FilterOperatorType, object, bool, FilterOperatorType, object) | Filtre une liste avec des critères personnalisés. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomFilter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomFilter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomFilter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomFilter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomFilter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomFilter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomFilter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomFilter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomFilter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCustomFilterCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Numbers");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["A4"].PutValue(30);
            sheet.Cells["A5"].PutValue(40);
            sheet.Cells["A6"].PutValue(50);

            // Activer d'abord le filtre automatique
            sheet.AutoFilter.Range = "A1:A6";
            
            // Créer des filtres personnalisés
            sheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, "30");
            sheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, "40");

            // Obtenir les filtres via la réflexion car la méthode directe n'est pas disponible
            var filterField = sheet.AutoFilter.GetType().GetField("m_customFilters", 
                System.Reflection.BindingFlags.NonPublic | System.Reflection.BindingFlags.Instance);
            var filters = (CustomFilterCollection)filterField.GetValue(sheet.AutoFilter);

            // Appliquer les filtres
            Cells_Type_CustomFilterCollection(sheet, filters);

            // Enregistrez le classeur
            workbook.Save("CustomFilterDemo.xlsx");
        }

        private static void Cells_Type_CustomFilterCollection(Worksheet sheet, CustomFilterCollection filters)
        {
            Console.WriteLine("Applying custom filters:");
            if (filters != null)
            {
                for (int i = 0; i < filters.Count; i++)
                {
                    Console.WriteLine($"Filter: {filters[i].FilterOperatorType}, Criteria: {filters[i].Criteria}");
                }
            }
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [CustomFilter](../customfilter/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


