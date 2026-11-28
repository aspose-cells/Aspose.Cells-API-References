---
title: "Column.Width"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Column özelliği. Sütun genişliğini karakter biriminde alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/column/width/
---
## Column.Width property

Sütun genişliğini karakter biriminde alır ve ayarlar.

```csharp
public double Width { get; set; }
```

### Açıklamalar

Elektronik tablo için sütun genişliği, normal stilin yazı tipinde 0~9 sayılarının maksimum rakam genişliğinin karakter sayısı olarak ölçülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sütun 3 için (indeks 2) genişliği ayarla
            worksheet.Cells.Columns[2].Width = 25.5;
            
            // Sütun 4 için (indeks 3) genişliği ayarla
            worksheet.Cells.Columns[3].Width = 40.0;
            
            // Genişlikleri al ve göster
            Console.WriteLine("Column 3 Width: " + worksheet.Cells.Columns[2].Width);
            Console.WriteLine("Column 4 Width: " + worksheet.Cells.Columns[3].Width);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ColumnWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


