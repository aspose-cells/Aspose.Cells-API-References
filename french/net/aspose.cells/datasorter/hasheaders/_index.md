---
title: "DataSorter.HasHeaders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorter. Indique si la plage a des en-têtes"
type: docs
url: /fr/net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

Représente si la plage possède des en-têtes.

```csharp
public bool HasHeaders { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyHasHeadersDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des en-têtes et des données d'exemple
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["B4"].PutValue(12);

            // Créer un trieur de données et définir HasHeaders sur true
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true; // This tells the sorter the first row contains headers
            
            // Trier par la première colonne (Fruits) en ordre croissant
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Trier la plage de données (en incluant les en-têtes)
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "B4"));

            // Enregistrer le classeur trié
            workbook.Save("SortedWithHeaders.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


