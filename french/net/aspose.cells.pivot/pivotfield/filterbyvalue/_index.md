---
title: "PivotField.FilterByValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Filtre par valeurs du champ pivot de données"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/filterbyvalue/
---
## PivotField.FilterByValue method

Filtre par valeurs du champ pivot de données.

```csharp
public PivotFilter FilterByValue(int valueFieldIndex, PivotFilterType type, double value1, 
    double value2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
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

    public class PivotFieldMethodFilterByValueWithInt32PivotFilterTypeDoubleDoubDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["B3"].Value = 1.8;
            worksheet.Cells["B4"].Value = 3.2;
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["C2"].Value = 100;
            worksheet.Cells["C3"].Value = 150;
            worksheet.Cells["C4"].Value = 80;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Ajouter des champs de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Appeler la méthode FilterByValue avec les paramètres (Int32, PivotFilterType, Double, Double)
                // Filtrer les produits où Quantity (indice du champ 1) est compris entre 90 et 160
                PivotFilter filter = pivotField.FilterByValue(1, PivotFilterType.ValueBetween, 90.0, 160.0);

                Console.WriteLine("FilterByValue method executed successfully");
                Console.WriteLine($"Filter type: {filter.FilterType}");
                Console.WriteLine($"Value field index: {filter.ValueFieldIndex}");

                // Actualisez le tableau croisé dynamique pour afficher les modifications
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FilterByValue method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("PivotFieldMethodFilterByValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


