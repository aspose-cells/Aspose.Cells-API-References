---
title: "Worksheet.GetSelectedRanges"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Tasarımcı elektronik tablosundaki seçili hücre aralıklarını alır"
type: docs
url: /tr/net/aspose.cells/worksheet/getselectedranges/
---
## Worksheet.GetSelectedRanges method

Tasarım elektronik tablosundaki seçili hücre aralıklarını alır.

```csharp
[Obsolete("Use Worksheet.GetSelectedAreas() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetSelectedRanges()
```

### Dönüş Değeri

Seçili aralıkları içeren bir ArrayList.

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine lütfen Worksheet.GetSelectedAreas() yöntemini kullanın. Bu özellik, Mart 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class WorksheetMethodGetSelectedRangesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "Test Value";

            try
            {
                // Not: GetSelectedRanges yansıma içinde kullanımdan kaldırılmış olarak işaretlenmiştir
                // Bu, istenildiği gibi yöntem çağrısını gösterir
                ArrayList selectedRanges = worksheet.GetSelectedRanges();

                // Seçili aralıkların sayısını göster
                Console.WriteLine($"Number of selected ranges: {selectedRanges.Count}");

                // Her bir seçili aralığı göster
                foreach (var range in selectedRanges)
                {
                    Console.WriteLine($"Selected range: {range}");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("GetSelectedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


