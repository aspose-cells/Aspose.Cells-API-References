---
title: "HeaderFooterCommand.Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HeaderFooterCommand özelliği. Komutun değerinin yazı tipini alır."
type: docs
url: /tr/net/aspose.cells/headerfootercommand/font/
---
## HeaderFooterCommand.Font property

Komutun değerinin yazı tipini alır.

```csharp
public Font Font { get; }
```

### Açıklamalar

HeaderFooterCommandType.Picture için işe yaramaz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HeaderFooterCommandPropertyFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Üstbilgi/altbilgi için sayfa ayarına erişin.
            PageSetup pageSetup = worksheet.PageSetup;

            // HeaderFooterCommand içerecek bir metinle üstbilgi ayarlayın.
            pageSetup.SetHeader(0, "&\"Arial\"&12&BThis is a header");

            // Üstbilgi betiğini al.
            string headerScript = pageSetup.GetHeader(0);

            // Üstbilgi komutlarını al
            HeaderFooterCommand[] commands = pageSetup.GetCommands(headerScript);

            // Metin komutunu bulun (ilk komut olduğunu varsayarak).
            if (commands.Length > 0 && commands[0].Type == HeaderFooterCommandType.Text)
            {
                HeaderFooterCommand textCommand = commands[0];
                
                // Font özelliğine erişin (yalnızca okunabilir).
                Font font = textCommand.Font;
                
                // Mevcut yazı tipi özelliklerini göster.
                Console.WriteLine("Current Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");

                // Font yalnızca okunabilir olduğu için yeni bir Font nesnesi atayamıyoruz,
                // ancak mevcut fontun özelliklerini değiştirebiliriz.
                font.Name = "Times New Roman";
                font.Size = 14;
                font.IsBold = false;
                font.Color = System.Drawing.Color.Blue;

                // Değişiklikleri görmek için çalışma kitabını kaydedin
                workbook.Save("HeaderFooterFontDemo.xlsx");

                Console.WriteLine("\nModified Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../font/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


