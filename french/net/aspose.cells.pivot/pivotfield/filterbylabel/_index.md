---
title: "PivotField.FilterByLabel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotField method. Filtre par les légendes du champ pivot de ligne ou de colonne"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/filterbylabel/
---
## PivotField.FilterByLabel method

Filtre par légendes du champ pivot de ligne ou de colonne.

```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | PivotFilterType | Le type de données de filtrage. |
| label1 | String | L'étiquette de la condition de filtre |
| label2 | String | L'étiquette supérieure de la condition de filtre entre |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByLabelWithPivotFilterTypeStringStringDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("");
            sheet.Cells["A5"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // Créer un tableau croisé dynamique avec les paramètres corrects
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Obtenez le champ du tableau croisé
            PivotField field = pivot.RowFields[0];
            
            // Appliquer les filtres
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotFilterByLabelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


