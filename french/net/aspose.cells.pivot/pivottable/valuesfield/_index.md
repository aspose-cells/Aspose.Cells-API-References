---
title: "PivotTable.ValuesField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient un objet PivotField qui représente tous les champs de données d'un tableau croisé dynamique. Lecture seule. Il ne sera créé que lorsqu'il y a deux champs de données ou plus dans la région Données. Par défaut, il se trouve dans la région des lignes. Vous pouvez le faire glisser vers la région ligne/colonne avec la méthode PivotTable.AddFieldToArea."
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/valuesfield/
---
## PivotTable.ValuesField property

Obtient un objet [`PivotField`](../../pivotfield/) qui représente tous les champs de données d'un tableau croisé dynamique. Lecture seule. Il ne sera créé que lorsqu'il y a deux champs de données ou plus dans la région Données. Par défaut, il se trouve dans la région des lignes. Vous pouvez le faire glisser vers la région ligne/colonne avec la méthode PivotTable.AddFieldToArea().

```csharp
public PivotField ValuesField { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyValuesFieldDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["A4"].PutValue("Product A");
            worksheet.Cells["B4"].PutValue("South");
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["A5"].PutValue("Product B");
            worksheet.Cells["B5"].PutValue("North");
            worksheet.Cells["C5"].PutValue(1200);

            try
            {
                // Créer un tableau croisé dynamique
                int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Ajouter des champs aux zones
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Calculer les données pour remplir le tableau croisé dynamique
                pivotTable.CalculateData();

                // Accéder à la propriété ValuesField (lecture seule)
                PivotField valuesField = pivotTable.ValuesField;

                if (valuesField != null)
                {
                    Console.WriteLine("ValuesField Name: " + valuesField.Name);
                    Console.WriteLine("ValuesField DisplayName: " + valuesField.DisplayName);
                    Console.WriteLine("ValuesField Position: " + valuesField.Position);
                    Console.WriteLine("ValuesField RegionType: " + valuesField.RegionType);
                    Console.WriteLine("ValuesField IsValuesField: " + valuesField.IsValuesField);
                }
                else
                {
                    Console.WriteLine("ValuesField is null - no data fields in the pivot table");
                }

                // Enregistrez le classeur
                workbook.Save("PivotTableValuesFieldDemo.xlsx");
                Console.WriteLine("PivotTable with ValuesField demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


