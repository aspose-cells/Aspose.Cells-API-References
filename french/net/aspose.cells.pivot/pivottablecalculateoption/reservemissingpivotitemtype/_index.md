---
title: "PivotTableCalculateOption.ReserveMissingPivotItemType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTableCalculateOption. Représente comment réserver les éléments manquants du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/
---
## PivotTableCalculateOption.ReserveMissingPivotItemType property

Représente la façon de réserver les éléments manquants du tableau croisé dynamique.

```csharp
public ReserveMissingPivotItemType ReserveMissingPivotItemType { get; set; }
```

### Remarques

Ne fonctionne que lorsque [`RefreshData`](../refreshdata/) est vrai.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyReserveMissingPivotItemTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(30);

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Configurer les champs du tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Définir les options de calcul avec ReserveMissingPivotItemType
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculer avec des options
            pivotTable.CalculateData(options);

            // Enregistrer le résultat
            workbook.Save("PivotTableReserveMissingItemsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ReserveMissingPivotItemType](../../reservemissingpivotitemtype/)
* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


