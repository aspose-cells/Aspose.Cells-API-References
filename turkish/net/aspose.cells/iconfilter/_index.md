---
title: "Sınıf IconFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.IconFilter sınıfı. Simge filtresini temsil eder"
type: docs
url: /tr/net/aspose.cells/iconfilter/
---
## IconFilter class

Simge filtresini temsil eder.

```csharp
public class IconFilter
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IconId](../../aspose.cells/iconfilter/iconid/) { get; set; } | Bir simge kümesindeki sıfır tabanlı simge indeksini alır ve ayarlar. |
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | Bu filtre ölçütü için kullanılan simge kümesini alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Örnek verileri doldur
                for (int i = 0; i < 10; i++)
                {
                    worksheet.Cells[i, 0].PutValue(i * 10);
                }

                // Otomatik filtre oluştur
                worksheet.AutoFilter.Range = "A1:A10";
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.IconFilter;

                // Simge filtresini al
                IconFilter iconFilter = (IconFilter)filterColumn.Filter;

                // Simge filtresi özelliklerini ayarla
                iconFilter.IconSetType = IconSetType.Arrows3;
                iconFilter.IconId = 1; // Filter for middle arrow

                Console.WriteLine($"IconFilter created with IconSetType: {iconFilter.IconSetType} and IconId: {iconFilter.IconId}");

                // Çalışma kitabını kaydedin
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon filter applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with IconFilter: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


