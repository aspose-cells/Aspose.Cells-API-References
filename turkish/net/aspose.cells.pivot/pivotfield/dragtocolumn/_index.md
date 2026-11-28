---
title: "PivotField.DragToColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer true'dur."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/dragtocolumn/
---
## PivotField.DragToColumn property

Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

```csharp
[Obsolete("Use PivotField.AllowDraggingToColumn property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToColumn { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.AllowDraggingToColumn özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToColumnDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Item");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(8);

            // Bir pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("=A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloya alan ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Veri alanını alın ve DragToColumn değerini true olarak ayarlayın.
            PivotField quantityField = pivotTable.DataFields[0];
            quantityField.DragToColumn = true; // This allows the field to be dragged to column area
            quantityField.DisplayName = "Total Quantity";

            // Verileri hesaplayın ve kaydedin
            pivotTable.CalculateData();
            workbook.Save("PivotFieldDragToColumnDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


