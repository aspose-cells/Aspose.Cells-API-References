---
title: "PivotTable.ShowRowHeaderCaption"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Satır başlığı etiketinin PivotTable raporunda gösterilip gösterilmediğini belirtir. Alan başlıklarını ve filtre açılır menülerini gösterip göstermediğini belirtir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showrowheadercaption/
---
## PivotTable.ShowRowHeaderCaption property

Satır başlığı etiketinin PivotTable raporunda gösterilip gösterilmediğini ve alan başlıkları ile filtre açılır menülerinin gösterilip gösterilmediğini belirtir

```csharp
[Obsolete("Use PivotTable.ShowHeaders property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowRowHeaderCaption { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotTable.ShowHeaders özelliğini kullanın. Bu yöntem, Nisan 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle ve örnek veri ile doldur
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Özet tablo için örnek veri ekle
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Pivot tabloyu yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // ShowRowHeaderCaption özelliğini göster
            pivotTable.ShowRowHeaderCaption = true;
            Console.WriteLine("Row Header Caption Visible: " + pivotTable.ShowRowHeaderCaption);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableShowRowHeaderCaptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


