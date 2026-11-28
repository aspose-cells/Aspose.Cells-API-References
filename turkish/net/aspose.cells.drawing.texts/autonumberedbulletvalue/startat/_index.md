---
title: "AutoNumberedBulletValue.StartAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoNumberedBulletValue özelliği. Madde işaretinin başlangıç numarasını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/autonumberedbulletvalue/startat/
---
## AutoNumberedBulletValue.StartAt property

Madde işaretinin başlangıç numarasını alır ve ayarlar.

```csharp
public int StartAt { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyStartAtDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Bir AutoNumberedBulletValue örneği oluştur.
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.ArabicPeriod,
                    StartAt = 3 // Setting the StartAt property
                };

                // Mevcut StartAt değerini göster
                Console.WriteLine($"Initial StartAt value: {bullet.StartAt}");

                // StartAt değerini değiştir
                bullet.StartAt = 5;
                Console.WriteLine($"Modified StartAt value: {bullet.StartAt}");

                // Bağlam içinde madde işaretini göstermek için bir şekil oluştur
                var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "1. First Item\n2. Second Item";

                // Madde işareti stilini uygula (not: gerçek uygulama yöntemi yansıtma içinde gösterilmemiştir)
                // Demonstrasyon amacıyla, sadece çalışma kitabını kaydedeceğiz
                workbook.Save("StartAtPropertyDemo.xlsx");
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

* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


