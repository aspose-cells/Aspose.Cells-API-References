---
title: "PivotItem.GetDoubleValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotItem. Obtient la valeur double de l'élément du tableau croisé. Si la valeur est nulle ou n'est pas un nombre, elle renverra 0"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/getdoublevalue/
---
## PivotItem.GetDoubleValue method

Obtient la valeur double de l'élément pivot. Si la valeur est nulle ou n'est pas un nombre, elle renverra 0

```csharp
public double GetDoubleValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetDoubleValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            foreach (PivotItem pivotItem in pivotItems)
            {
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);
                double doubleValue = pivotItem.GetDoubleValue();
                Console.WriteLine("Double Value: " + doubleValue);
            }

            workbook.Save("PivotItemGetDoubleValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


