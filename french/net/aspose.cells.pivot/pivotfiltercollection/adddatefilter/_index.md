---
title: "PivotFilterCollection.AddDateFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotFilterCollection. Filtre par le paramètre de date du champ pivot de ligne ou de colonne"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfiltercollection/adddatefilter/
---
## PivotFilterCollection.AddDateFilter method

Filtre par paramètre de date du champ pivot de ligne ou de colonne.

```csharp
public PivotFilter AddDateFilter(int baseFieldIndex, PivotFilterType type, DateTime dateTime1, 
    DateTime dateTime2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | L'index du champ dans la source. |
| type | PivotFilterType | Le type de données de filtrage. |
| dateTime1 | DateTime | L'étiquette de date de la condition de filtre |
| dateTime2 | DateTime | L'étiquette de date supérieure de la condition de filtre entre |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddDateFilterWithInt32PivotFilterTypeDateTimeDaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec des dates
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

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
                
                // Ajouter un filtre de date pour afficher les dates entre le 1 janv. et le 31 mar. 2023
                PivotFilter filter = filters.AddDateFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.DateBetween,
                    dateTime1: new DateTime(2023, 1, 1),
                    dateTime2: new DateTime(2023, 3, 31)
                );

                Console.WriteLine($"Date filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, UseWholeDay: {filter.UseWholeDay}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding date filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddDateFilterDemo.xlsx");
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


