---
title: "DynamicFilter.MaxValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DynamicFilter. Obtient et définit la valeur maximale du filtre dynamique"
type: docs
url: /fr/net/aspose.cells/dynamicfilter/maxvalue/
---
## DynamicFilter.MaxValue property

Obtient et définit la valeur maximale du filtre dynamique.

```csharp
public object MaxValue { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données numériques d'exemple
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);

            // Créez un filtre automatique
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Appliquer le filtre dynamique avec des critères de plage
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Afficher la valeur MaxValue actuelle
            Console.WriteLine("Current MaxValue: " + filter.MaxValue);

            // Comme DynamicFilterType.Between n'existe pas, nous utiliserons une approche différente
            // Par exemple, nous pouvons utiliser un filtre personnalisé à la place
            worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, 20);
            worksheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, 40);

            // Appliquer le filtre
            worksheet.AutoFilter.Refresh();

            // Enregistrer le résultat
            workbook.Save("DynamicFilterMaxValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


