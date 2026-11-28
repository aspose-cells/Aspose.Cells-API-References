---
title: "Range.ColumnWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Bu aralığın sütun genişliğini ayarlar veya alır"
type: docs
url: /tr/net/aspose.cells/range/columnwidth/
---
## Range.ColumnWidth property

Bu aralığın sütun genişliğini ayarlar veya alır

```csharp
public double ColumnWidth { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralığa (B ile D sütunları) erişin
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B:D");
            
            // Mevcut sütun genişliğini gösterin
            Console.WriteLine("Current ColumnWidth: " + range.ColumnWidth);

            // Yeni sütun genişliğini ayarlayın (karakter biriminde)
            range.ColumnWidth = 15.0;

            // Etkiyi göstermek için hücreleri doldurun
            worksheet.Cells["B1"].PutValue("This is column B");
            worksheet.Cells["C1"].PutValue("This is column C");
            worksheet.Cells["D1"].PutValue("This is column D");

            // İçeriği göstermek için satırları otomatik sığdır
            worksheet.AutoFitRows();

            // Çalışma kitabını kaydedin
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


