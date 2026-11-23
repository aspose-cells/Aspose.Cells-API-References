---
title: "PivotDiscreteGroupSettings.Items"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotDiscreteGroupSettings. Obtient les éléments discrets"
type: docs
url: /fr/net/aspose.cells.pivot/pivotdiscretegroupsettings/items/
---
## PivotDiscreteGroupSettings.Items property

Obtient les éléments discrets.

```csharp
[Obsolete("Use PivotField.GroupBy(DiscreteGroupItem[], bool) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomPiovtFieldGroupItem[] Items { get; }
```

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.GroupBy(DiscreteGroupItem[], bool). Cette méthode sera supprimée 12 mois plus tard à compter de juillet 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDiscreteGroupSettingsPropertyItemsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Apple");
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(150);
            worksheet.Cells["B6"].PutValue(250);

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Obtenir le champ pivot et le regrouper
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[0], false);

            // Accéder aux paramètres du groupe discret
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Afficher les éléments actuels
            Console.WriteLine("Current Items count: " + groupSettings.Items.Length);
            foreach (CustomPiovtFieldGroupItem item in groupSettings.Items)
            {
                Console.WriteLine("Item: " + item.ToString());
            }

            // Enregistrez le classeur
            workbook.Save("PivotDiscreteGroupSettingsItemsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


