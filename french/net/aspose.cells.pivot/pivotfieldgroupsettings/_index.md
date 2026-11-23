---
title: "Classe PivotFieldGroupSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotFieldGroupSettings. Représente le paramètre de groupe du champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldgroupsettings/
---
## PivotFieldGroupSettings class

Représente le paramètre de groupe du champ de tableau croisé dynamique.

```csharp
public class PivotFieldGroupSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PivotFieldGroupSettings](pivotfieldgroupsettings/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [Type](../../aspose.cells.pivot/pivotfieldgroupsettings/type/) { get; } | Obtient le type de groupe du champ pivot. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsDemo
    {
        public static void PivotFieldGroupSettingsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Amount";
            worksheet.Cells[1, 1].Value = 50;
            worksheet.Cells[2, 1].Value = 60;
            worksheet.Cells[3, 1].Value = 70;
            worksheet.Cells[4, 1].Value = 80;

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Accédez au champ de ligne
            PivotField rowField = pivotTable.RowFields[0];
            rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);

            // Accédez aux paramètres de groupe du champ de ligne
            PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

            // Affiche le type de groupe du champ pivot
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Enregistrez le classeur
            workbook.Save("PivotFieldGroupSettingsExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


