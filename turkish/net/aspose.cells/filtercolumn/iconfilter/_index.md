---
title: "FilterColumn.IconFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Verileri simgeye göre filtrelemek için IconFilter alır"
type: docs
url: /tr/net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

`IconFilter` alır; verileri simgeye göre filtrelemek için.

```csharp
public IconFilter IconFilter { get; }
```

### Açıklamalar

Bu özelliği kullanmadan önce, lütfen [`FilterType`](../filtertype/) değerinin IconFilter olduğundan emin olun, aksi takdirde null dönecektir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Simgeleri kullanan koşullu biçimlendirme ile örnek veri ekleyin
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // Aralığa otomatik filtre uygula
                worksheet.AutoFilter.Range = "A1:A5";

                // Filtre sütununu alın
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // IconFilter özelliğine erişin (yalnızca okunur)
                IconFilter iconFilter = filterColumn.IconFilter;

                // Var ise IconFilter özelliklerini göster
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


