---
title: "SubtotalSetting.GroupBy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SubtotalSetting özelliği. Gruplandırılacak alan, sıfır tabanlı bir tam sayı offseti olarak"
type: docs
url: /tr/net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

Gruplamak için alan, sıfır‑tabanlı bir tam sayı ofseti olarak

```csharp
public int GroupBy { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SubtotalSettingPropertyGroupByDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Group A");
            worksheet.Cells["A3"].PutValue("Group B");
            worksheet.Cells["A4"].PutValue("Group A");
            worksheet.Cells["A5"].PutValue("Group B");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(400);

            try
            {
                // Alt toplamlar için hücre alanını tanımlayın
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Veriye alt toplamları uygulayın
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // GroupBy özelliğine erişmek için alt toplam ayarını alın
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // GroupBy özelliği değerini göster
                Console.WriteLine("GroupBy field index: " + subtotalSetting.GroupBy);

                // Çalışma kitabını kaydedin
                workbook.Save("GroupByDemo.xlsx");
                Console.WriteLine("Subtotal with GroupBy demonstrated successfully.");
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

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


