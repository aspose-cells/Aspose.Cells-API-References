---
title: "DynamicFilter.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DynamicFilter. Obtient et définit la valeur du filtre dynamique"
type: docs
url: /fr/net/aspose.cells/dynamicfilter/value/
---
## DynamicFilter.Value property

Obtient et définit la valeur du filtre dynamique.

```csharp
public object Value { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            // Créez un filtre automatique
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Affichez la valeur actuelle du filtre
            Console.WriteLine("Current DynamicFilter Value: " + filter.Value);

            // Modifiez la valeur du filtre pour afficher les dates d'avril
            filter.Value = new DateTime(2023, 4, 1);
            filter.DynamicFilterType = DynamicFilterType.April;

            // Appliquer le filtre
            worksheet.AutoFilter.Refresh();

            // Enregistrer le résultat
            workbook.Save("DynamicFilterValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


