---
title: "PivotTable.BaseFields"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Retourne tous les champs pivot de base dans le PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/basefields/
---
## PivotTable.BaseFields property

Renvoie tous les champs pivot de base du PivotTable.

```csharp
public PivotFieldCollection BaseFields { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyBaseFieldsDemo
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
            worksheet.Cells["A5"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Actualiser les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Accéder à la collection BaseFields
            PivotFieldCollection baseFields = pivotTable.BaseFields;
            
            // Afficher les éléments originaux de chaque champ de base
            Console.WriteLine("Base Fields and their Original Items:");
            foreach (PivotField field in baseFields)
            {
                Console.WriteLine($"Field: {field.Name}");
                string[] originalItems = field.OriginalItems;
                foreach (string item in originalItems)
                {
                    Console.WriteLine($"- {item}");
                }
            }
        }
    }
}
```

### Voir aussi

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


