---
title: "Cells.GetViewRowHeightInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen bir satırın yüksekliğini inç biriminde alır"
type: docs
url: /tr/net/aspose.cells/cells/getviewrowheightinch/
---
## Cells.GetViewRowHeightInch method

Belirtilen bir satırın yüksekliğini inç biriminde alır.

```csharp
public double GetViewRowHeightInch(int row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi |

### Dönüş Değeri

Satır yüksekliği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetViewRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır 2 için inç cinsinden özel satır yüksekliği ayarla
            worksheet.Cells.SetRowHeightInch(2, 1.5);

            try
            {
                // Satır indeks parametresiyle GetViewRowHeightInch metodunu çağır
                double rowHeight = worksheet.Cells.GetViewRowHeightInch(2);
                
                // Sonucu göster ve yüksekliğin ayarlanan değerle eşleştiğini doğrula
                Console.WriteLine($"View row height of row 2: {rowHeight} inches");
                
                // Örnek içerik ekleyerek etkiyi göster
                worksheet.Cells["A2"].PutValue($"Row Height: {rowHeight}\"");
                worksheet.Cells.SetColumnWidthInch(0, 15);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetViewRowHeightInch: {ex.Message}");
            }
            
            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("CellsMethodGetViewRowHeightInchWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


