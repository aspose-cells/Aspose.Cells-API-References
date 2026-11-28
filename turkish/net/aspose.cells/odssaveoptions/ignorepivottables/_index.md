---
title: "OdsSaveOptions.IgnorePivotTables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsSaveOptions özelliği. Özet tabloların kaydedilip kaydedilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/odssaveoptions/ignorepivottables/
---
## OdsSaveOptions.IgnorePivotTables property

Özet tabloların kaydedilip kaydedilmeyeceğini gösterir.

```csharp
public bool IgnorePivotTables { get; set; }
```

### Açıklamalar

OpenOffice'in özet tablo özelliği, Excel'e kıyasla daha az ayara sahiptir, bu nedenle özet tablo sonuçları birçok farklılık gösterir. Bazen .ods dosyası kaydedilirken bu özet tabloları görmezden gelmek daha iyidir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Bir pivot tablo oluştur
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // OdsSaveOptions örneği oluştur
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Mevcut IgnorePivotTables değerini göster
            Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);

            // Kaydederken özet tabloları görmezden gelmek için ayarla
            saveOptions.IgnorePivotTables = true;

            // Özet tablolar görmezden gelinerek kaydet
            workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);

            // Kaydederken özet tabloları dahil etmek için ayarla
            saveOptions.IgnorePivotTables = false;

            // Özet tablolar dahil edilerek kaydet
            workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


