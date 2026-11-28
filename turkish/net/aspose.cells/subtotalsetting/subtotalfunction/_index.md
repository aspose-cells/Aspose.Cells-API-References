---
title: "SubtotalSetting.SubtotalFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SubtotalSetting özelliği. Alt toplam işlevi"
type: docs
url: /tr/net/aspose.cells/subtotalsetting/subtotalfunction/
---
## SubtotalSetting.SubtotalFunction property

Alt toplam işlevi.

```csharp
public ConsolidationFunction SubtotalFunction { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySubtotalFunctionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Mevcut veriden alarak alt toplam ayarı oluştur
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Alt toplamı yapılandır - bu özellikler gerçek API'de yalnızca okunabilir
            // Bu yüzden Subtotal yöntemini parametrelerle doğrudan kullanacağız
            int groupBy = 0; // Group by first column
            ConsolidationFunction function = ConsolidationFunction.Sum;
            int[] subtotalColumns = new int[] {1}; // Subtotal on second column
            
            // Alt toplamları uygula
            worksheet.Cells.Subtotal(area, groupBy, function, subtotalColumns);

            // Alınan ayardan SubtotalFunction özelliğini doğrula
            Console.WriteLine("Subtotal Function: " + subtotalSetting.SubtotalFunction);
            
            // Çalışma kitabını kaydedin
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


