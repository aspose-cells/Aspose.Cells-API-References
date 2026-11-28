---
title: "Range.ColumnCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Aralıktaki sütun sayısını alır"
type: docs
url: /tr/net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Aralıktaki sütun sayısını alır.

```csharp
public int ColumnCount { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri oluşturun (5 sütun x 3 satır)
            for (int col = 0; col < 5; col++)
            {
                for (int row = 0; row < 3; row++)
                {
                    sheet.Cells[row, col].PutValue($"Data {row},{col}");
                }
            }
            
            // Tüm veri sütunlarını kapsayan bir aralık oluşturun
            Aspose.Cells.Range dataRange = sheet.Cells.CreateRange(0, 0, 3, 5);
            
            // ColumnCount kullanımını gösterin
            Console.WriteLine($"Range has {dataRange.ColumnCount} columns");
            
            // Aralıktaki her sütunu otomatik olarak sığdırın
            for (int i = 0; i < dataRange.ColumnCount; i++)
            {
                sheet.AutoFitColumn(dataRange.FirstColumn + i);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


