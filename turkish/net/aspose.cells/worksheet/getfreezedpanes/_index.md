---
title: "Worksheet.GetFreezedPanes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Dondurulmuş bölmeleri alır"
type: docs
url: /tr/net/aspose.cells/worksheet/getfreezedpanes/
---
## Worksheet.GetFreezedPanes method

Donma bölmelerini alır.

```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows, 
    out int freezedColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32& | Satır indeksi. |
| sütun | Int32& | Sütun indeksi. |
| freezedRows | Int32& | Üst bölmede görünen satır sayısı, satır indeksinden fazla olamaz. |
| freezedColumns | Int32& | Sol bölmede görünen sütun sayısı, sütun indeksinden fazla olamaz. |

### Dönüş Değeri

Çalışma sayfasının dondurulmuş olup olmadığını döndürür

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodGetFreezedPanesWithInt32ParametersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // C5 hücresinde (satır 4, sütun 2) 2 dondurulmuş satır ve 1 dondurulmuş sütunla bölmeleri dondur
            worksheet.FreezePanes(4, 2, 2, 1);

            // Dondurulmuş bölme bilgilerini saklamak için değişkenleri bildir
            int row = 0;
            int column = 0;
            int freezedRows = 0;
            int freezedColumns = 0;

            try
            {
                // GetFreezedPanes yöntemini çıkış parametreleriyle çağır
                bool hasFreeze = worksheet.GetFreezedPanes(out row, out column, out freezedRows, out freezedColumns);

                // Sonuçları görüntüleyin
                Console.WriteLine("Worksheet has freeze panes: " + hasFreeze);
                if (hasFreeze)
                {
                    Console.WriteLine("Freeze position - Row: " + row + ", Column: " + column);
                    Console.WriteLine("Frozen rows: " + freezedRows + ", Frozen columns: " + freezedColumns);
                }

                // Çalışma kitabını kaydedin
                workbook.Save("WorksheetMethodGetFreezedPanesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFreezedPanes method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


