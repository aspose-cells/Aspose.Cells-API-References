---
title: "PivotFilterCollection.AddLabelFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotFilterCollection. Filtre par les légendes de la ligne ou de la colonne du champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfiltercollection/addlabelfilter/
---
## PivotFilterCollection.AddLabelFilter method

Filtre par légendes du champ pivot de ligne ou de colonne.

```csharp
public PivotFilter AddLabelFilter(int baseFieldIndex, PivotFilterType type, string label1, 
    string label2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | L'index du champ dans la source. |
| type | PivotFilterType | Le type de données de filtrage. |
| label1 | String | L'étiquette de la condition de filtre |
| label2 | String | L'étiquette supérieure de la condition de filtre entre |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddLabelFilterWithInt32PivotFilterTypeStringStriDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Cherry";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

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
                
                // Ajouter un filtre d'étiquette pour afficher les produits commençant par "A"
                PivotFilter filter = filters.AddLabelFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.CaptionBeginsWith,
                    label1: "A",
                    label2: null
                );

                Console.WriteLine($"Label filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value1: {filter.Value1}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding label filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddLabelFilterDemo.xlsx");
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


