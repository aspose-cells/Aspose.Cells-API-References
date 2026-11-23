---
title: "Worksheet.AutoFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Représente le filtre automatique pour la feuille de calcul spécifiée"
type: docs
url: /fr/net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

Représente le filtre automatique pour la feuille de calcul spécifiée.

```csharp
public AutoFilter AutoFilter { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Shirt");
            worksheet.Cells["B3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Phone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["A5"].PutValue("Pants");
            worksheet.Cells["B5"].PutValue("Clothing");

            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.Filter(1, "Electronics");

            // Actualiser le filtre
            worksheet.AutoFilter.Refresh();

            // Enregistrez le classeur
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


