---
title: "FilterColumn.Filter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Verileri filtreleme koşulunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/filtercolumn/filter/
---
## FilterColumn.Filter property

Verileri filtreleme koşulunu alır ve ayarlar.

```csharp
[Obsolete("Use corresponding property according to the filter type instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Filter { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, lütfen [`FilterType`](../filtertype/) göre ilgili özelliği kullanın. Ve filtre türü MultipleFilters için, döndürülen nesne artık [`FilterValueCollection`](../../filtervaluecollection/) yerine [`MultipleFilterCollection`](../../multiplefiltercollection/) olur. Bu özellik Ekim 2025'ten itibaren 12 ay içinde kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Renk biçimlendirmeli örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Color");
            cells["A2"].PutValue("Red");
            cells["A3"].PutValue("Red");
            cells["A4"].PutValue("Blue");
            
            // Hücreleri renklerle biçimlendir
            Style redStyle = workbook.CreateStyle();
            redStyle.ForegroundColor = Color.Red;
            redStyle.Pattern = BackgroundType.Solid;
            
            Style blueStyle = workbook.CreateStyle();
            blueStyle.ForegroundColor = Color.Blue;
            blueStyle.Pattern = BackgroundType.Solid;
            
            cells["A2"].SetStyle(redStyle);
            cells["A3"].SetStyle(redStyle);
            cells["A4"].SetStyle(blueStyle);
            
            // Otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Kırmızı hücreler için renk filtresi ekle
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Filtre sütununa ve onun Filter özelliğine eriş
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            // Filtre özelliklerini çıktıla
            Console.WriteLine($"Filter type: {fc.FilterType}");
            Console.WriteLine($"Filter by fill color: {cf.FilterByFillColor}");
            Console.WriteLine($"Filter color: {cf.GetColor(workbook.Worksheets)}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("ColorFilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


