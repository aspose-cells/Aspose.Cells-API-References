---
title: "PivotTable.IsAutoFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si le rapport du tableau croisé dynamique est formaté automatiquement. Case à cocher autoformatage du tableau qui se trouve dans l'option pivottable pour Excel 2003"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/isautoformat/
---
## PivotTable.IsAutoFormat property

Indique si le rapport du tableau croisé dynamique est formaté automatiquement. Case à cocher "autoformat table" qui se trouve dans les options du tableau croisé dynamique pour Excel 2003.

```csharp
public bool IsAutoFormat { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsAutoFormatDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // Ajouter un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Définir la propriété IsAutoFormat
            pivotTable.IsAutoFormat = true; // Enable auto formatting
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotTableIsAutoFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


