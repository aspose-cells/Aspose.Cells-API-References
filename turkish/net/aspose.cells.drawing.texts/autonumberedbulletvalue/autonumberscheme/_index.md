---
title: "AutoNumberedBulletValue.AutonumberScheme"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoNumberedBulletValue özelliği. Otomatik numaranın şemasını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/
---
## AutoNumberedBulletValue.AutonumberScheme property

Otomatik numaranın şemasını temsil eder.

```csharp
public TextAutonumberScheme AutonumberScheme { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyAutonumberSchemeDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir AutoNumberedBulletValue örneği oluştur
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue();

                // İlk AutonumberScheme değerini göster
                Console.WriteLine($"Default AutonumberScheme: {bullet.AutonumberScheme}");

                // Yeni bir AutonumberScheme değeri ayarla
                bullet.AutonumberScheme = TextAutonumberScheme.RomanUcPeriod;
                Console.WriteLine($"Modified AutonumberScheme: {bullet.AutonumberScheme}");

                // Madde işaretini bağlam içinde göstermek için bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Madde işareti stilini kullanacak metin içeren bir şekil oluştur
                TextBox shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "Sample text with bullet formatting";


                // Not: Madde işareti stilinin metne uygulanması ek API çağrıları gerektirir
                // Yansıma içinde gösterilmemiştir. Sadece bir gösterim olarak çalışma kitabını kaydedeceğiz.
                workbook.Save("AutonumberSchemeDemo.xlsx");
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

* enum [TextAutonumberScheme](../../textautonumberscheme/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


