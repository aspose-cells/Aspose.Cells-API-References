---
title: "HeaderFooterCommand.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HeaderFooterCommand özelliği. Komutun metnini alır."
type: docs
url: /tr/net/aspose.cells/headerfootercommand/text/
---
## HeaderFooterCommand.Text property

Komutun metnini alır.

```csharp
public string Text { get; }
```

### Açıklamalar

Yalnızca HeaderFooterCommandType.Text için geçerlidir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Metin komutuyla üstbilgi ayarlayın.
            worksheet.PageSetup.SetHeader(1, "&\"Arial\"&12&KFF0000Sample Text Header");
            
            // Üstbilgi komutlarını al
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(worksheet.PageSetup.GetHeader(1));
            
            // Metin komutu hakkında bilgi göster.
            foreach (HeaderFooterCommand cmd in commands)
            {
                if (cmd.Type == HeaderFooterCommandType.Text)
                {
                    Console.WriteLine("Text command found:");
                    Console.WriteLine("Text: " + cmd.Text);
                    Console.WriteLine("Font: " + cmd.Font);
                    Console.WriteLine("Color: " + ColorTranslator.ToHtml(cmd.Font.Color));
                }
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("HeaderFooterTextDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


