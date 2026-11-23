---
title: "Classe DynamicFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DynamicFilter. Représente le filtre dynamique"
type: docs
url: /fr/net/aspose.cells/dynamicfilter/
---
## DynamicFilter class

Représente le filtre dynamique.

```csharp
public class DynamicFilter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | Obtient et définit le type de ce filtre dynamique. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | Obtient et définit la valeur maximale du filtre dynamique. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | Obtient et définit la valeur du filtre dynamique. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un classeur et une feuille de calcul (facultatif pour le contexte)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Name = "DemoSheet";

                // Remplir avec des données numériques d'exemple
                worksheet.Cells["A1"].PutValue("Numbers");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);
                worksheet.Cells["A6"].PutValue(50);

                // Définir une plage d'autofilter
                worksheet.AutoFilter.Range = "A1:A6";

                // Appliquer un filtre dynamique (AboveAverage) à la première colonne
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);

                // Récupérer l'instance DynamicFilter créée par l'AutoFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Définir des propriétés supplémentaires si désiré
                filter.Value = 25;      // Example custom value
                filter.MaxValue = 45;   // Example max value

                // Afficher les propriétés définies
                Console.WriteLine($"DynamicFilterType: {filter.DynamicFilterType}");
                Console.WriteLine($"Value: {filter.Value}");
                Console.WriteLine($"MaxValue: {filter.MaxValue}");

                // Actualiser le filtre pour appliquer les modifications
                worksheet.AutoFilter.Refresh();

                // Enregistrer le classeur (les données filtrées seront enregistrées)
                workbook.Save("DynamicFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DynamicFilter: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


