---
title: "AutoNumberedBulletValue.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoNumberedBulletValue özelliği. Madde işaretinin tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/autonumberedbulletvalue/type/
---
## AutoNumberedBulletValue.Type property

Madde işaretinin türünü alır.

```csharp
public override BulletType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Madde işaretli metin eklemek için bir şekil oluştur
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 10, 300, 100);
            var textParagraph = shape.TextBody.TextParagraphs[0];

            // Otomatik numaralı bir madde işareti değeri oluştur
            var bullet = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.AlphaLcParenBoth,
                StartAt = 1
            };

            // BulletValue'yu doğrudan ayarlayamadığımız için başka bir yol bulmamız gerekecek
            // madde işareti stilini uygulamak için. Bu, şeklin metin biçimlendirmesini kullanmayı içerebilir
            // veya API'de mevcut diğer yöntemler.
            // Demonstrasyon amacıyla, sadece madde işareti tipini göstereceğiz
            Console.WriteLine("Bullet Type: " + bullet.Type);

            // Şeklin metin gövdesi aracılığıyla paragrafa metin ekle
            shape.TextBody.Text = "First Item";

            // Farklı bir numaralandırma şemasıyla başka bir paragraf ekle
            // Ekleyemediğimiz için, bir sonraki kullanılabilir paragrafı kullanacağız
            var secondParagraph = shape.TextBody.TextParagraphs[1];
            var bullet2 = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.Arabic1Minus,
                StartAt = 1
            };

            // Madde işareti tipini göster (yalnızca okunabilir özellik)
            Console.WriteLine("Second Bullet Type: " + bullet2.Type);

            // İkinci paragrafın içine metin ekle
            shape.TextBody.Text += "\nSecond Item";

            // Madde işareti etkilerini göstermek için çalışma kitabını kaydet
            workbook.Save("AutoNumberedBulletDemo.xlsx");
        }
    }

}
```

### Ayrıca Bakınız

* enum [BulletType](../../bullettype/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


