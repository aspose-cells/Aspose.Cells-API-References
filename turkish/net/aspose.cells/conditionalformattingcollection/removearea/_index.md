---
title: "ConditionalFormattingCollection.RemoveArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConditionalFormattingCollection yöntemi. Aralıktaki tüm koşullu biçimlendirmeleri kaldırın"
type: docs
url: /tr/net/aspose.cells/conditionalformattingcollection/removearea/
---
## ConditionalFormattingCollection.RemoveArea method

Aralıktaki tüm koşullu biçimlendirmeleri kaldır.

```csharp
public void RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Aralığın başlangıç satırı. |
| startColumn | Int32 | Aralığın başlangıç sütunu. |
| totalRows | Int32 | Aralıktaki satır sayısı. |
| totalColumns | Int32 | Aralıktaki sütun sayısı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Koşullu biçimlendirme koleksiyonunu alın
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;

            // Bazı koşullu biçimlendirme kuralları ekleyin
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddArea(area);

            try
            {
                // RemoveArea metodunu (Int32, Int32, Int32, Int32) parametreleriyle çağırın
                cfc.RemoveArea(0, 0, 3, 3);

                Console.WriteLine("Conditional formatting removed from area (0,0,3,3)");
                
                // Etkisini sayıyı kontrol ederek doğrulayın (tüm biçimlendirme kaldırıldıysa bu 0 olur)
                Console.WriteLine($"Remaining conditional formatting areas: {fcc.RangeCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("RemoveAreaWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


