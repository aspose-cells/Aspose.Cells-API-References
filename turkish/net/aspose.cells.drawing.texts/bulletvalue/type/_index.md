---
title: "BulletValue.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BulletValue özelliği. Mermi değerinin türünü alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/bulletvalue/type/
---
## BulletValue.Type property

Madde işaretinin değerinin tipini alır.

```csharp
public abstract BulletType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class BulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Bir metin kutusu oluştur ve metin paragraflarını al
                var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var textParagraph = textBox.TextBody.TextParagraphs[0];

                // BulletValue'den türetilen bir karakter mermi değeri oluştur
                var bulletValue = new CharacterBulletValue();
                bulletValue.Character = '•';

                // Type özelliği değerini gösterin
                Console.WriteLine("Bullet Type: " + bulletValue.Type);

                // Farklı türü göstermek için bir resim mermi değeri oluştur
                var pictureBullet = new PictureBulletValue();
                Console.WriteLine("Picture Bullet Type: " + pictureBullet.Type);

                // Çalışma kitabını kaydedin
                workbook.Save("BulletValueTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


