---
title: "FilterColumnCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "FilterColumnCollection propriété. Obtient l'objet FilterColumn au champ spécial."
type: docs
url: /fr/net/aspose.cells/filtercolumncollection/item/
---
## FilterColumnCollection indexer

Obtient l'objet [`FilterColumn`](../../filtercolumn/) au champ spécial.

```csharp
public FilterColumn this[int fieldIndex] { get; }
```

| Paramètre | Description |
| --- | --- |
| fieldIndex | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |

### Valeur de retour

Renvoie l'objet [`FilterColumn`](../../filtercolumn/).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["A5"].PutValue("Date");

            // Appliquer le filtre automatique
            sheet.AutoFilter.Range = "A1:A5";
            sheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "e");

            // Accédez au filtre en utilisant la propriété Item
            AutoFilter filter = sheet.AutoFilter;
            FilterColumn filterColumn = filter.FilterColumns[0]; // Using Item property
            CustomFilterCollection customFilters = (CustomFilterCollection)filterColumn.Filter;
            CustomFilter firstFilter = customFilters[0];

            // Affiche les propriétés du filtre
            Console.WriteLine("Filter Operator Type: " + firstFilter.FilterOperatorType);
            Console.WriteLine("Filter Criteria: " + firstFilter.Criteria);

            // Modifiez le filtre
            firstFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("\nModified Filter Operator Type: " + firstFilter.FilterOperatorType);

            // Enregistrez le classeur
            wb.Save("FilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


