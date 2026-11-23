---
title: "Énumération PivotLineType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Pivot.PivotLineType. Spécifie le type du PivotLine"
type: docs
url: /fr/net/aspose.cells.pivot/pivotlinetype/
---
## PivotLineType enumeration

Spécifie le type de la PivotLine.

```csharp
public enum PivotLineType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Regular | `0` | PivotLine régulier avec des éléments pivot. |
| Subtotal | `1` | Ligne de sous-total. |
| GrandTotal | `2` | Ligne du total général. |
| Blank | `3` | Ligne vide après chaque groupe. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotLineTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Trier le champ de ligne par valeurs en ordre décroissant
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "B2");
            
            // Calculer les données du tableau croisé dynamique
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotLineTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


