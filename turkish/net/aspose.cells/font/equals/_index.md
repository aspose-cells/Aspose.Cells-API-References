---
title: "Font.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font yöntemi. İki yazı tipinin eşit olup olmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells/font/equals/
---
## Font.Equals method

İki yazı tipinin eşit olup olmadığını denetler.

```csharp
public bool Equals(Font font)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yazı tipi | Yazı Tipi | Karşılaştırılan yazı tipi nesnesi. |

### Dönüş Değeri

Karşılaştırılan yazı tipi nesnesine eşitse doğru.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontMethodEqualsWithFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karşılaştırmak için iki yazı tipi nesnesi oluşturun
            Font font1 = workbook.CreateStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            font1.IsBold = true;
            font1.Color = System.Drawing.Color.Black;

            Font font2 = workbook.CreateStyle().Font;
            font2.Name = "Arial";
            font2.Size = 12;
            font2.IsBold = true;
            font2.Color = System.Drawing.Color.Black;

            try
            {
                // Yazı tiplerini karşılaştırmak için Equals yöntemini çağırın
                bool areEqual = font1.Equals(font2);

                // Sonucu göster
                Console.WriteLine($"The fonts are equal: {areEqual}");

                // Farklı olmalarını sağlamak için bir yazı tipini değiştirin
                font2.IsItalic = true;
                areEqual = font1.Equals(font2);
                Console.WriteLine($"After modification, the fonts are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("FontEqualsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


