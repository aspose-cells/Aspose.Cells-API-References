---
title: "Enum NumberCategoryType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.NumberCategoryType enum. Hücrelerin sayı biçimlendirme kategorisi türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/numbercategorytype/
---
## NumberCategoryType enumeration

Hücrenin sayı biçimlendirmesinin kategori türünü temsil eder.

```csharp
public enum NumberCategoryType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| General | `0` | Genel |
| Text | `1` | Metin |
| Number | `2` | Sayı |
| Date | `3` | Tarih veya Tarih ve Saat |
| Time | `4` | Saat |
| Fraction | `5` | Kesir |
| Scientific | `6` | Bilimsel |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NumberCategoryTypeDemo
    {
        public static void NumberCategoryTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("General");
            worksheet.Cells["A2"].PutValue("Text");
            worksheet.Cells["A3"].PutValue(12345);
            worksheet.Cells["A4"].PutValue(DateTime.Now);
            worksheet.Cells["A5"].PutValue(TimeSpan.FromHours(1.5));
            worksheet.Cells["A6"].PutValue(0.75);
            worksheet.Cells["A7"].PutValue(1.23E+3);

            // Hücreler için sayı biçimlerini ayarla
            worksheet.Cells["A1"].SetStyle(CreateStyle(workbook, NumberCategoryType.General));
            worksheet.Cells["A2"].SetStyle(CreateStyle(workbook, NumberCategoryType.Text));
            worksheet.Cells["A3"].SetStyle(CreateStyle(workbook, NumberCategoryType.Number));
            worksheet.Cells["A4"].SetStyle(CreateStyle(workbook, NumberCategoryType.Date));
            worksheet.Cells["A5"].SetStyle(CreateStyle(workbook, NumberCategoryType.Time));
            worksheet.Cells["A6"].SetStyle(CreateStyle(workbook, NumberCategoryType.Fraction));
            worksheet.Cells["A7"].SetStyle(CreateStyle(workbook, NumberCategoryType.Scientific));

            // Sayı kategori türlerini çıktıla
            Console.WriteLine("Cell A1 Number Category Type: " + worksheet.Cells["A1"].NumberCategoryType);
            Console.WriteLine("Cell A2 Number Category Type: " + worksheet.Cells["A2"].NumberCategoryType);
            Console.WriteLine("Cell A3 Number Category Type: " + worksheet.Cells["A3"].NumberCategoryType);
            Console.WriteLine("Cell A4 Number Category Type: " + worksheet.Cells["A4"].NumberCategoryType);
            Console.WriteLine("Cell A5 Number Category Type: " + worksheet.Cells["A5"].NumberCategoryType);
            Console.WriteLine("Cell A6 Number Category Type: " + worksheet.Cells["A6"].NumberCategoryType);
            Console.WriteLine("Cell A7 Number Category Type: " + worksheet.Cells["A7"].NumberCategoryType);

            // Çalışma kitabını kaydedin
            workbook.Save("NumberCategoryTypeExample.xlsx");
        }

        private static Style CreateStyle(Workbook workbook, NumberCategoryType numberCategoryType)
        {
            Style style = workbook.CreateStyle();
            switch (numberCategoryType)
            {
                case NumberCategoryType.General:
                    style.Number = 0;
                    break;
                case NumberCategoryType.Text:
                    style.Number = 49;
                    break;
                case NumberCategoryType.Number:
                    style.Number = 1;
                    break;
                case NumberCategoryType.Date:
                    style.Number = 14;
                    break;
                case NumberCategoryType.Time:
                    style.Number = 21;
                    break;
                case NumberCategoryType.Fraction:
                    style.Number = 9;
                    break;
                case NumberCategoryType.Scientific:
                    style.Number = 11;
                    break;
            }
            return style;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


