---
title: "Range.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Aralığı yapıştırma özel seçenekleriyle kopyalama"
type: docs
url: /tr/net/aspose.cells/range/copy/
---
## Copy(Range, PasteOptions) {#copy_1}

Aralığı özel yapıştırma seçenekleriyle kopyalama.

```csharp
public void Copy(Range range, PasteOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Aralık | Kaynak aralık. |
| seçenekler | PasteOptions | Yapıştırma özel seçenekleri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangePasteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Kaynak aralıkta örnek veri oluştur
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Tam nitelikli tip ile aralıklar oluştur
            Aspose.Cells.Range source = sheet.Cells.CreateRange(0, 0, 5, 5);
            Aspose.Cells.Range destination = sheet.Cells.CreateRange(6, 0, 5, 5);

            // Yapıştırma seçeneklerini ayarla
            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            // Yapıştırma seçenekleriyle kopyala
            destination.Copy(source, options);

            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Range) {#copy}

Kaynak bir aralıktan veri (formüller dahil), biçimlendirme, çizim nesneleri vb. kopyalar.

```csharp
public void Copy(Range range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | Range | Kaynak [`Range`](../) nesnesi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Kaynak ve hedef aralıklar oluştur
            Aspose.Cells.Range sourceRange = cells.CreateRange("A1:A5");
            Aspose.Cells.Range destRange = cells.CreateRange("A6:A10");
            
            // Kaynak aralığı örnek veriyle doldur
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue($"Data {i + 1}");
            }
            
            // Kaynak aralığı hedefe kopyala
            sourceRange.Copy(destRange);
            
            workbook.Save("RangeCopyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


