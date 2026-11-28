---
title: "Enum TextOrientationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TextOrientationType enum. Metin yönlendirme türlerini listeler"
type: docs
url: /tr/net/aspose.cells/textorientationtype/
---
## TextOrientationType enumeration

Metin yönlendirme türlerini listeler.

```csharp
public enum TextOrientationType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| ClockWise | `0` | Metni saat yönünde 90 derece döndürür. |
| CounterClockWise | `1` | Metni saat yönünün tersine 90 derece döndürür. |
| NoRotation | `2` | Varsayılan değeri temsil eder. |
| TopToBottom | `3` | Metni hücrenin üstünden altına gösterir. Yığılmış metin. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextOrientationTypeDemo
    {
        public static void TextOrientationTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");
            worksheet.Cells["A2"].PutValue("This is a test comment.");

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add(0, 0);
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment with text orientation.";

            // Yorum için farklı metin yönlendirme türlerini ayarla
            comment.TextOrientationType = TextOrientationType.ClockWise;
            Console.WriteLine("Text Orientation: ClockWise");

            // Çalışma kitabını kaydedin
            workbook.Save("TextOrientationTypeExample_ClockWise.xlsx");

            // Metin yönlendirmesini CounterClockWise olarak değiştir
            comment.TextOrientationType = TextOrientationType.CounterClockWise;
            Console.WriteLine("Text Orientation: CounterClockWise");

            // Çalışma kitabını kaydedin
            workbook.Save("TextOrientationTypeExample_CounterClockWise.xlsx");

            // Metin yönlendirmesini NoRotation olarak değiştir
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Text Orientation: NoRotation");

            // Çalışma kitabını kaydedin
            workbook.Save("TextOrientationTypeExample_NoRotation.xlsx");

            // Metin yönlendirmesini TopToBottom olarak değiştir
            comment.TextOrientationType = TextOrientationType.TopToBottom;
            Console.WriteLine("Text Orientation: TopToBottom");

            // Çalışma kitabını kaydedin
            workbook.Save("TextOrientationTypeExample_TopToBottom.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


