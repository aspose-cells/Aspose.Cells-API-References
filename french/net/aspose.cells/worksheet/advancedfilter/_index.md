---
title: "Worksheet.AdvancedFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Filtre les données en utilisant des critères complexes"
type: docs
url: /fr/net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

Filtre les données en utilisant des critères complexes.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isFilter | Boolean | Indique si le filtrage de la liste se fait sur place. |
| listRange | String | La plage de la liste. |
| criteriaRange | String | La plage de critères. |
| copyTo | String | La plage où copier les données. |
| uniqueRecordOnly | Boolean | Affichage ou copie uniquement des lignes uniques. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAdvancedFilterWithBooleanStringStringStringBooleDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le filtrage
            // En-têtes
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            // Critères
            worksheet.Cells["A2"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Category");
            worksheet.Cells["C2"].PutValue("Fruits");
            
            // Données
            worksheet.Cells["A4"].PutValue("Apple");
            worksheet.Cells["B4"].PutValue("Fruits");
            worksheet.Cells["C4"].PutValue(2.5);
            
            worksheet.Cells["A5"].PutValue("Carrot");
            worksheet.Cells["B5"].PutValue("Vegetables");
            worksheet.Cells["C5"].PutValue(1.2);
            
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B6"].PutValue("Fruits");
            worksheet.Cells["C6"].PutValue(1.8);

            // Appliquer le filtre avancé (filtrer sur place, uniquement les enregistrements uniques)
            worksheet.AdvancedFilter(false, "A4:C6", "A1:C2", null, true);

            // Enregistrez le classeur
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


