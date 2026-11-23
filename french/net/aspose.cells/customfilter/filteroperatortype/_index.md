---
title: "CustomFilter.FilterOperatorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CustomFilter. Obtient et définit le type d'opérateur de filtre"
type: docs
url: /fr/net/aspose.cells/customfilter/filteroperatortype/
---
## CustomFilter.FilterOperatorType property

Obtient et définit le type d'opérateur de filtre.

```csharp
public FilterOperatorType FilterOperatorType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Mike");
            worksheet.Cells["A5"].PutValue("Emily");

            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Appliquer le filtre personnalisé avec l'opérateur Contains
            filter.Custom(0, FilterOperatorType.Contains, "e");
            
            // Obtenir le premier filtre personnalisé
            CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
            
            // Démontrer la propriété FilterOperatorType
            Console.WriteLine("Initial Filter Operator: " + customFilter.FilterOperatorType);
            Console.WriteLine("Criteria: " + customFilter.Criteria);
            
            // Modifier le type d'opérateur de filtre
            customFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
            
            // Enregistrez le classeur
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


