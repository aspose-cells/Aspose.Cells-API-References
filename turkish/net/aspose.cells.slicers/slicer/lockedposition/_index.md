---
title: "Slicer.LockedPosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Slicer özelliği. Belirtilen dilimleyicinin kullanıcı arayüzü kullanılarak taşınıp taşınamayacağını veya yeniden boyutlandırılıp yeniden boyutlandırılamayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.slicers/slicer/lockedposition/
---
## Slicer.LockedPosition property

Belirtilen slicerin kullanıcı arabirimi kullanılarak taşınıp yeniden boyutlandırılıp yapılamayacağını gösterir.

```csharp
public bool LockedPosition { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedPositionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Özet tablo koleksiyonu oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Bir pivot tablo oluştur
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Dilimleyici koleksiyonu oluştur
            SlicerCollection slicers = worksheet.Slicers;
            
            // Özet tablo için bir dilimleyici ekle
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];

            // Dilimleyici özelliklerini ayarla
            slicer.Caption = "Fruit Slicer";
            slicer.NumberOfColumns = 2;
            slicer.WidthPixel = 200;
            slicer.HeightPixel = 150;

            // LockedPosition özelliğini göster
            slicer.LockedPosition = true; // Lock the slicer position
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Hareket etmeye izin vermek için LockedPosition değerini false yap
            slicer.LockedPosition = false;
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Çalışma kitabını kaydedin
            workbook.Save("SlicerLockedPositionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


