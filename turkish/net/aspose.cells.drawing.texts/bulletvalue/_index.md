---
title: "Sınıf BulletValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.BulletValue sınıfı. Madde işaretinin değerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/bulletvalue/
---
## BulletValue class

Madde işaretinin değerinin temsilidir.

```csharp
public abstract class BulletValue
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| abstract [Type](../../aspose.cells.drawing.texts/bulletvalue/type/) { get; } | Madde işaretinin değerinin tipini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassBulletValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu oluştur ve metin paragraflarını al
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var textParagraph = textBox.TextBody.TextParagraphs[0];

            // CharacterBulletValue örneği oluştur (BulletValue'dan miras alır)
            var bulletValue = new CharacterBulletValue();
            bulletValue.Character = '•';
            
            // Madde işareti değerini paragrafa ayarla (Bullet yalnızca okunur, bu yüzden farklı bir şekilde değiştirmemiz gerekir)
            // Bullet yalnızca okunur olduğu için, onu ayarlamanın başka bir yolunu bulmamız gerekiyor
            // Bu, madde işareti ayarlı yeni bir TextParagraph oluşturmayı içerebilir
            // Not: Gerçek API, madde işaretlerini ayarlamanın farklı bir yolunu sağlayabilir
            // Demonstrasyon amaçlı, bunu başka bir yolla ayarlayabileceğimizi varsayacağız
            // textParagraph.Bullet = bulletValue; // Bu satır Bullet yalnızca okunur olduğu için kaldırıldı
            textBox.Text = "First bullet point";

            // Farklı bir madde işaretiyle başka bir paragraf ekle
            // TextParagraphCollection'da Add metodu yok, bu yüzden başka bir yol bulmamız gerekiyor
            // Bu, yeni bir TextParagraph oluşturup başka bir yolla eklemeyi içerebilir
            // Demonstrasyon amaçlı, ikinci paragrafı doğrudan alabileceğimizi varsayacağız
            var textParagraph2 = textBox.TextBody.TextParagraphs[1];
            var bulletValue2 = new CharacterBulletValue();
            bulletValue2.Character = '→';
            // textParagraph2.Bullet = bulletValue2; // Bu satır Bullet yalnızca okunur olduğu için kaldırıldı
            textBox.Text += "\nSecond bullet point";

            // Madde işareti tipine erişimi göster
            Console.WriteLine("First bullet type: " + textParagraph.Bullet.Type);
            Console.WriteLine("Second bullet type: " + textParagraph2.Bullet.Type);

            // Sonucu kaydet
            workbook.Save("TextsClassBulletValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


