---
title: "Name.GetRanges"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name yöntemi. Bu ad tarafından başvurulan tüm aralıkları alır"
type: docs
url: /tr/net/aspose.cells/name/getranges/
---
## GetRanges() {#getranges}

Bu ad tarafından referans verilen tüm aralıkları alır.

```csharp
public Range[] GetRanges()
```

### Dönüş Değeri

Tüm aralıklar.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            
            // Adlandırılmış bir aralık oluştur
            int index = workbook.Worksheets.Names.Add("Fruits");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Yeniden hesaplamalı aralıkları al
            Aspose.Cells.Range[] ranges1 = name.GetRanges();
            Console.WriteLine("Ranges with recalculation:");
            PrintRanges(ranges1);
            
            // Yeniden hesaplamasız aralıkları al
            Aspose.Cells.Range[] ranges2 = name.GetRanges(false);
            Console.WriteLine("\nRanges without recalculation:");
            PrintRanges(ranges2);
        }
        
        private static void PrintRanges(Aspose.Cells.Range[] ranges)
        {
            if (ranges != null)
            {
                foreach (Aspose.Cells.Range range in ranges)
                {
                    Console.WriteLine($"Range: {range.Address}");
                }
            }
            else
            {
                Console.WriteLine("No ranges found");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRanges(bool) {#getranges_1}

Bu ad tarafından referans verilen tüm aralıkları alır.

```csharp
public Range[] GetRanges(bool recalculate)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yeniden hesapla | Boolean | Bu ad bu çağrıdan önce hesaplandıysa yeniden hesaplayıp hesaplamama. |

### Dönüş Değeri

Tüm aralıklar.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesWithBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Adlandırılmış bir aralık oluştur
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Yeniden hesaplamadan aralıkları al
            Aspose.Cells.Range[] ranges1 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count (no recalc): " + ranges1.Length);
            
            // Yeniden hesaplayarak aralıkları al
            Aspose.Cells.Range[] ranges2 = namedRange.GetRanges();
            Console.WriteLine("Ranges count (with recalc): " + ranges2.Length);
            
            // Aralığı değiştir ve yeniden hesaplamayı göster
            worksheet.Cells["A4"].PutValue(30);
            namedRange.RefersTo = "=Sheet1!$A$1:$A$4";
            
            // Değişiklikten sonra yeniden hesaplayarak ve yeniden hesaplamadan aralıkları al
            Aspose.Cells.Range[] ranges3 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count after mod (no recalc): " + ranges3.Length);
            
            Aspose.Cells.Range[] ranges4 = namedRange.GetRanges();
            Console.WriteLine("Ranges count after mod (with recalc): " + ranges4.Length);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


