---
title: "CustomFilter.Criteria"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CustomFilter. Obtient et définit les critères"
type: docs
url: /fr/net/aspose.cells/customfilter/criteria/
---
## CustomFilter.Criteria property

Obtient et définit les critères.

```csharp
public object Criteria { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Numbers");
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(5);
            worksheet.Cells["A5"].PutValue(9);
            worksheet.Cells["A6"].PutValue(3);

            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:A6";
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Ajouter un filtre personnalisé
            int fieldIndex = 0;
            autoFilter.Custom(fieldIndex, FilterOperatorType.GreaterOrEqual, 5);
            
            // Obtenir la colonne du filtre et afficher les critères
            FilterColumn fc = autoFilter.FilterColumns[fieldIndex];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Console.WriteLine("Filter Criteria: " + cf.Criteria);
            
            // Actualiser le filtre
            autoFilter.Refresh();
            
            // Enregistrez le classeur
            workbook.Save("CustomFilterExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


