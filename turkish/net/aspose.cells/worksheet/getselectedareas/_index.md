---
title: "Worksheet.GetSelectedAreas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Tasarımcı elektronik tablosundaki seçili hücre aralıklarını alır"
type: docs
url: /tr/net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

Tasarım elektronik tablosundaki seçili hücre aralıklarını alır.

```csharp
public Range[] GetSelectedAreas()
```

### Dönüş Değeri

Tüm seçili aralıkları döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetSelectedAreasDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Birden fazla aralık seç
            worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
            worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
            
            // Seçili alanları al
            Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
            
            // Seçili alanlar hakkında bilgi göster
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            for (int i = 0; i < selectedAreas.Length; i++)
            {
                Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
            }
            
            // Seçimleri temizle ve tek bir aralık seç
            worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
            
            // Tek seçili alanı al
            selectedAreas = worksheet.GetSelectedAreas();
            Console.WriteLine("\nAfter single selection:");
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            Console.WriteLine("Selected area: " + selectedAreas[0].Address);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


