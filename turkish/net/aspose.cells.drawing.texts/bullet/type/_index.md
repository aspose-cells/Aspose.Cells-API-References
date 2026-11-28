---
title: "Bullet.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Bullet özelliği. Madde işaretinin tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/bullet/type/
---
## Bullet.Type property

Bullet tipini alır ve ayarlar.

```csharp
public BulletType Type { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class BulletPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu ekle
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            // Madde işareti özelliklerini yapılandır
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character; // Demonstrating Type property usage
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Çalışma kitabını kaydedin
            workbook.Save("BulletPropertyTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


