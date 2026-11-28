---
title: "FilterType enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FilterType enum. Filtre türü"
type: docs
url: /tr/net/aspose.cells/filtertype/
---
## FilterType enumeration

Filtre türü.

```csharp
public enum FilterType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| ColorFilter | `0` | Hücrenin dolgu rengine göre filtrele. |
| CustomFilters | `1` | Özel filtre türü. |
| DynamicFilter | `2` | Dinamik filtre türü. |
| MultipleFilters | `3` | Filtrelemek için birden fazla değer seçildiğinde veya bir grup tarih değeri seçildiğinde, bu öğe bu kriterleri bir araya toplar. |
| IconFilter | `4` | Koşullu biçimlendirme simgesine göre filtrele. |
| Top10 | `5` | İlk 10 filtre. |
| None | `6` | Filtre yok. |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Color");
            worksheet.Cells["A2"].PutValue("Red");
            worksheet.Cells["A3"].PutValue("Green");
            worksheet.Cells["A4"].PutValue("Blue");
            
            // Otomatik filtre oluştur
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Renk filtresi oluşturun
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            
            // Sütuna renk filtresi ekleyin
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Filtre türünü kontrol edin
            FilterColumn filterColumn = filter.FilterColumns[0];
            Console.WriteLine("Filter Type: " + filterColumn.FilterType);
            
            // Renk filtresi özelliklerini doğrulayın
            if (filterColumn.FilterType == FilterType.ColorFilter)
            {
                ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
                Console.WriteLine("Filter by fill color: " + colorFilter.FilterByFillColor);
                Console.WriteLine("Filter color: " + colorFilter.GetColor(workbook.Worksheets));
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


