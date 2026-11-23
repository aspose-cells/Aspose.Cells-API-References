---
title: "PivotTable.DataField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient un objet PivotField qui représente tous les champs de données d'un tableau croisé dynamique. Lecture seule. Il ne sera créé que lorsqu'il y a deux champs de données ou plus dans la région Données. Par défaut, il se trouve dans la région des lignes. Vous pouvez le faire glisser vers la région ligne/colonne avec la méthode PivotTable.AddFieldToArea."
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Obtient un objet [`PivotField`](../../pivotfield/) qui représente tous les champs de données d'un tableau croisé dynamique. Lecture seule. Il ne sera créé que lorsqu'il y a deux champs de données ou plus dans la région Données. Par défaut, il se trouve dans la région des lignes. Vous pouvez le faire glisser vers la région ligne/colonne avec la méthode PivotTable.AddFieldToArea().

```csharp
[Obsolete("Use PivotTable.ValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotField DataField { get; }
```

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.ValuesField. Cette méthode sera supprimée 12 mois plus tard, à compter d'octobre 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Accéder et modifier les propriétés DataField
            // La position est en lecture seule, nous allons donc démontrer d'autres propriétés
            pivotTable.DataField.DisplayName = "Total Sales";
            pivotTable.DataField.NumberFormat = "#,##0";
            
            // Enregistrez le classeur
            workbook.Save("PivotTableDataFieldDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


