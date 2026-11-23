---
title: "PivotItem.GetDateTimeValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotItem. Obtient la valeur date/heure de l'élément pivot. Si la valeur est nulle, elle renverra DateTime.MinValue"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/getdatetimevalue/
---
## PivotItem.GetDateTimeValue method

Obtient la valeur date/heure de l'élément pivot. Si la valeur est nulle, elle renverra DateTime.MinValue

```csharp
public DateTime GetDateTimeValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetDateTimeValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple avec une valeur de date
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            foreach (PivotItem pivotItem in pivotItems)
            {
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            workbook.Save("PivotItemGetDateTimeValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


