---
title: "PivotFieldSortSetting.FieldIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFieldSortSetting. Représente l’indice du champ utilisé pour le tri. 1 signifie trier le PivotField par les libellés, d’autres valeurs signifient trier par le champ de données"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldsortsetting/fieldindex/
---
## PivotFieldSortSetting.FieldIndex property

Représente l’indice du champ utilisé pour le tri. -1 signifie trier le PivotField par les libellés, d’autres valeurs signifient trier par le champ de données.

```csharp
[Obsolete("Use PivotFieldSortSetting.SortBy property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int FieldIndex { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotFieldSortSetting.SortBy. Cette méthode sera supprimée 12 mois après septembre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Obtenir le paramètre de tri du champ pivot
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;

            // Afficher la valeur actuelle de FieldIndex
            Console.WriteLine("Current FieldIndex value: " + sortSetting.FieldIndex);

            // Remarque : FieldIndex est en lecture seule et PivotFieldSortSetting ne peut pas être instancié directement
            // car il n’a aucun constructeur public. Nous ne pouvons travailler qu’avec l’instance existante
            // obtenue à partir de la propriété SortSetting du champ pivot.

            // Actualiser le tableau croisé dynamique pour appliquer les modifications
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrer le résultat
            workbook.Save("PivotFieldSortSettingFieldIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


