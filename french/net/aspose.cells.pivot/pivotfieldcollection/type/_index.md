---
title: "PivotFieldCollection.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFieldCollection. Obtient le type des PivotFields"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldcollection/type/
---
## PivotFieldCollection.Type property

Obtient le type des PivotFields.

```csharp
public PivotFieldType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Affiche le type de la collection de champs pivot
            Console.WriteLine("PivotFieldCollection Type: " + rowFields.Type);

            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotFieldCollection dataFields = pivotTable.DataFields;

            // Affiche le type de la collection de champs de données
            Console.WriteLine("DataFields Type: " + dataFields.Type);

            // Calculer les données et actualiser le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrer le résultat
            workbook.Save("PivotFieldCollectionTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


