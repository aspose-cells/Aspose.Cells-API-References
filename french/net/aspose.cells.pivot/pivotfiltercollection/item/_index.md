---
title: "PivotFilterCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFilterCollection. Obtient l'objet pivotfilter à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfiltercollection/item/
---
## PivotFilterCollection indexer

Obtient l'objet pivotfilter à l'index spécifique.

```csharp
public PivotFilter this[int index] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un filtre pivot en utilisant la méthode PivotFilterCollection.Add
            pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[0]; // Using Item property via index
            filter.Name = "SampleFilter";
            filter.Value1 = "100";
            
            // Accéder au filtre en utilisant la propriété Item et afficher les informations
            Console.WriteLine("Filter Name: " + pivotTable.PivotFilters[0].Name);
            Console.WriteLine("Filter Value1: " + pivotTable.PivotFilters[0].Value1);
            Console.WriteLine("Filter Type: " + pivotTable.PivotFilters[0].FilterType);
            
            // Enregistrez le classeur
            workbook.Save("PivotFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../../pivotfilter/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


