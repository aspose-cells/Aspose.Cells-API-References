---
title: "AutoFilter.DynamicFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Ajoute un filtre dynamique"
type: docs
url: /fr/net/aspose.cells/autofilter/dynamicfilter/
---
## AutoFilter.DynamicFilter method

Ajoute un filtre dynamique.

```csharp
public void DynamicFilter(int fieldIndex, DynamicFilterType dynamicFilterType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| dynamicFilterType | DynamicFilterType | Type de filtre dynamique. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodDynamicFilterWithInt32DynamicFilterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            // Appliquer le filtre automatique en utilisant la signature de méthode correcte
            worksheet.AutoFilter.Range = "A1:A6";

            // Appliquer le filtre dynamique pour les dates de mars
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            workbook.Save("DynamicFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


