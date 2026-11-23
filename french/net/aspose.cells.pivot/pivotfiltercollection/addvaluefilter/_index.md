---
title: "PivotFilterCollection.AddValueFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotFilterCollection. Filtre par les valeurs du champ pivot de données"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfiltercollection/addvaluefilter/
---
## PivotFilterCollection.AddValueFilter method

Filtre par valeurs du champ pivot de données.

```csharp
public PivotFilter AddValueFilter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    double value1, double value2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | L'index du champ dans la source. |
| valueFieldIndex | Int32 | L'index du champ de valeur dans la région de valeur. |
| type | PivotFilterType | Le type de données de filtrage. |
| value1 | Double | La valeur de la condition de filtre |
| value2 | Double | La valeur supérieure de la condition de filtre entre |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddValueFilterWithInt32Int32PivotFilterTypeDoublDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Widget";
            worksheet.Cells["A3"].Value = "Gadget";
            worksheet.Cells["A4"].Value = "Thingy";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 15.99;
            worksheet.Cells["B3"].Value = 24.99;
            worksheet.Cells["B4"].Value = 9.99;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Ajouter un filtre de valeur pour afficher les produits dont le prix est compris entre 10 $ et 20 $
                PivotFilter filter = filters.AddValueFilter(
                    baseFieldIndex: 0,
                    valueFieldIndex: 1,
                    type: PivotFilterType.ValueBetween,
                    value1: 10.0,
                    value2: 20.0
                );

                Console.WriteLine($"Value filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding value filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddValueFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


