---
title: "PivotField.DragToData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Belirtilen alanın değer bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer true'tur."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/dragtodata/
---
## PivotField.DragToData property

Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

```csharp
[Obsolete("Use PivotField.AllowDraggingToData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToData { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.AllowDraggingToData özelliğini kullanın. Bu yöntem Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri ekleyin.
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Bikes";
            cells["A4"].Value = "Cars";
            cells["A5"].Value = "Cars";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 1500;
            cells["C4"].Value = 2000;
            cells["C5"].Value = 2500;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanı ekleyin ve DragToData'yı yapılandırın
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];
            rowField.DragToData = true; // Allow dragging this field to data area
            
            // Sütun alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot tabloyu yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldDragToDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


