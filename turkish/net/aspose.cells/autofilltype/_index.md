---
title: "Enum AutoFillType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AutoFillType enum. Otomatik doldurma tipini temsil eder."
type: docs
url: /tr/net/aspose.cells/autofilltype/
---
## AutoFillType enumeration

Otomatik doldurma türünü temsil eder.

```csharp
public enum AutoFillType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Copy | `1` | Kaynak alanın değerini ve biçimini hedef alana kopyalar |
| Default | `0` | Hedef alanı değer ve biçimle otomatik olarak doldurur. |
| Formats | `3` | Kaynak alanın yalnızca biçimini hedef alana kopyalar. |
| Series | `2` | Kaynak alandaki değeri bir dizi şeklinde hedef alana genişlet ve biçimi hedef alana kopyala. |
| Values | `4` | Kaynak alanın yalnızca değerini hedef alana kopyalar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFillTypeDemo
    {
        public static void AutoFillTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1:A10 aralığını oluştur ve bazı değerlerle doldur
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A10");
            for (int i = 0; i < 10; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            // B1:B10 hedef aralığını oluştur
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B10");

            //Seri tipi hatası, bir bilet oluşturuldu
            // Hedef aralığı doldurmak için AutoFill metodunu AutoFillType.Series ile kullanın
            //sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // Hedef aralığı doldurmak için AutoFill metodunu AutoFillType.Copy ile kullanın
            sourceRange.AutoFill(targetRange, AutoFillType.Copy);
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFillTypeExample.xlsx");
            workbook.Save("AutoFillTypeExample.pdf");
        }
    }

}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


