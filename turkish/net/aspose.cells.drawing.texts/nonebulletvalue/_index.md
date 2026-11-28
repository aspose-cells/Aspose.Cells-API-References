---
title: "Sınıf NoneBulletValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.NoneBulletValue sınıfı. Hiç madde işareti temsil etmez"
type: docs
url: /tr/net/aspose.cells.drawing.texts/nonebulletvalue/
---
## NoneBulletValue class

Madde işareti olmadığını temsil eder.

```csharp
public class NoneBulletValue : BulletValue
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [NoneBulletValue](nonebulletvalue/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [Type](../../aspose.cells.drawing.texts/nonebulletvalue/type/) { get; } | Madde işaretinin değerinin tipini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class NoneBulletValueDemo
    {
        public static void NoneBulletValueExample()
        {
            // Yeni bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücreye metin ekleme
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text without bullet");

            // Madde işareti ayarlarını uygulamak için bir TextBox oluştur
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "This is a TextBox without bullet points";

            // NoneBulletValue örneği oluştur
            NoneBulletValue noneBulletValue = new NoneBulletValue();

            // Madde işaretinin tipini kontrol et (None olmalı)
            BulletType bulletType = noneBulletValue.Type;
            Console.WriteLine("Bullet Type: " + bulletType); // Output should be None

            // Değişiklikleri göstermek için çalışma kitabını kaydet
            workbook.Save("NoneBulletValueExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


