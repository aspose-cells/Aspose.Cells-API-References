---
title: "Sınıf HeaderFooterCommand"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HeaderFooterCommand sınıfı. Üst bilgi/alt bilgi komutunu temsil eder."
type: docs
url: /tr/net/aspose.cells/headerfootercommand/
---
## HeaderFooterCommand class

Üstbilgi/altbilgi komutunu temsil eder

```csharp
public class HeaderFooterCommand
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | Komutun değerinin yazı tipini alır. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | Komutun metnini alır. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | Üstbilgi/altbilgi komut türünü alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHeaderFooterCommandDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // PageSetup'a erişin ve komutlarla üstbilgi ayarlayın
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(1, "&D&\"Arial\"sdfsdfsdfsdf");
            
            // Üstbilgi komutlarını al
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(1));
            
            // Komut türlerini ve metni göster
            Console.WriteLine("Command 1 Type: " + commands[0].Type);
            Console.WriteLine("Command 2 Type: " + commands[1].Type);
            Console.WriteLine("Command 2 Text: " + commands[1].Text);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


