---
title: "PivotFieldGroupSettings.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFieldGroupSettings. Obtient le type de groupe du champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldgroupsettings/type/
---
## PivotFieldGroupSettings.Type property

Obtient le type de groupe du champ pivot.

```csharp
public virtual PivotFieldGroupType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            worksheet.Cells["A3"].Value = new DateTime(2023, 1, 2);
            worksheet.Cells["A4"].Value = new DateTime(2023, 1, 3);

            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Ajoutez un tableau croisé dynamique à la feuille de calcul
                int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "D3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Ajouter des champs au tableau croisé dynamique
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

                // Accéder au champ de ligne et regrouper par date
                PivotField rowField = pivotTable.RowFields[0];
                rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("DateGroup", new int[] { 0, 1 }) }, true);

                // Accédez aux paramètres de groupe du champ de ligne
                PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

                // Afficher la valeur actuelle de la propriété Type (lecture seule)
                Console.WriteLine("Pivot Field Group Type: " + groupSettings.Type);

                // Enregistrez le classeur
                workbook.Save("PivotFieldGroupSettingsTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
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

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotFieldGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


