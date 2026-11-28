---
title: "AutoFilter.Sorter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter özelliği. Veri sıralayıcısını alır"
type: docs
url: /tr/net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Veri sıralayıcısını alır.

```csharp
public DataSorter Sorter { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertySorterDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Otomatik filtre aralığını oluştur
            worksheet.AutoFilter.Range = "A1:B4";

            // Otomatik filtreyi al
            AutoFilter filter = worksheet.AutoFilter;

            // Filtreyi uygula
            filter.Filter(1, "10");

            // Sıralayıcı özelliğini kullanarak sırala
            filter.Sorter.Sort();

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFilterPropertySorterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


