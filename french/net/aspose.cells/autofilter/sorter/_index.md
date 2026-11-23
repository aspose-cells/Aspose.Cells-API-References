---
title: "AutoFilter.Sorter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoFilter. Obtient le trieur de données"
type: docs
url: /fr/net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Obtient le trieur de données.

```csharp
public DataSorter Sorter { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertySorterDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Créer une plage de filtre automatique
            worksheet.AutoFilter.Range = "A1:B4";

            // Obtenir le filtre automatique
            AutoFilter filter = worksheet.AutoFilter;

            // Appliquer le filtre
            filter.Filter(1, "10");

            // Trier en utilisant la propriété Sorter
            filter.Sorter.Sort();

            // Enregistrez le classeur
            workbook.Save("AutoFilterPropertySorterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


