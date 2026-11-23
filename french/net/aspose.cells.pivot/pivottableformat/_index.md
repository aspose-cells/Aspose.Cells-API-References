---
title: "Classe PivotTableFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotTableFormat. Représente le format défini dans le PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivottableformat/
---
## PivotTableFormat class

Représente le format défini dans le **PivotTable**.

```csharp
public class PivotTableFormat
```

## Propriétés

| Nom | Description |
| --- | --- |
| [PivotArea](../../aspose.cells.pivot/pivottableformat/pivotarea/) { get; } | Obtient la zone du pivot. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetStyle](../../aspose.cells.pivot/pivottableformat/getstyle/)() | Obtient le style formaté. |
| [SetStyle](../../aspose.cells.pivot/pivottableformat/setstyle/)(Style) | Définit le style de la zone du pivot. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableFormatDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Ajouter un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Accéder à la PivotTableFormatCollection
            PivotTableFormatCollection pivotFormats = pivotTable.PivotFormats;

            // Ajouter un nouveau format à la collection
            int formatIndex = pivotFormats.Add();
            PivotTableFormat pivotFormat = pivotFormats[formatIndex];

            // Accéder à la PivotArea du format
            PivotArea pivotArea = pivotFormat.PivotArea;
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Créer un nouveau style
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Appliquer le style au PivotTableFormat
            pivotFormat.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


