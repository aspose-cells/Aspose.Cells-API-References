---
title: "HeaderFooterCommand.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HeaderFooterCommand özelliği. Üstbilgi/altbilgi komut tipini alır."
type: docs
url: /tr/net/aspose.cells/headerfootercommand/type/
---
## HeaderFooterCommand.Type property

Üstbilgi/altbilgi komut türünü alır.

```csharp
public HeaderFooterCommandType Type { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Farklı komut tipleriyle başlık ayarla
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(0, "&D&\"Arial\"&12sdfsdfsdfsdf");
            
            // Üstbilgi komutlarını al
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(0));
            
            // Type özelliğinin kullanımını gösterin.
            Console.WriteLine("Command 0 Type: " + commands[0].Type); // CurrentDate
            Console.WriteLine("Command 1 Type: " + commands[1].Type); // Text
            Console.WriteLine("Command 1 Text: " + commands[1].Text); // sdfsdfsdfsdf
        }
    }
}
```

### Ayrıca Bakınız

* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


