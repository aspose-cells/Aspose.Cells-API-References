---
title: "PageSetup.GetCommands"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Üstbilgi veya altbilgi için tüm komutları alır"
type: docs
url: /tr/net/aspose.cells/pagesetup/getcommands/
---
## PageSetup.GetCommands method

Üst bilgi veya alt bilginin tüm komutlarını alır.

```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| headerFooterScript | String | Üstbilgi/altbilgi betiği |

### Dönüş Değeri

Üstbilgi veya altbilgi için tüm komutları döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetCommandsWithStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Üstbilgiyi komutlarla ayarla
            string header = "&D&\"Arial\"&12sdfsdfsdfsdf";
            worksheet.PageSetup.SetHeader(1, header);
            
            // Üstbilgi komutlarını al
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(header);
            
            // Komut türlerini ve metni göster
            foreach (HeaderFooterCommand cmd in commands)
            {
                Console.WriteLine($"Type: {cmd.Type}, Text: {cmd.Text}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


