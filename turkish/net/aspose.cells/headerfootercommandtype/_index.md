---
title: "Enum HeaderFooterCommandType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HeaderFooterCommandType enum. Başlık ve altbilgi komut tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

Üstbilgi ve altbilgi komut türünü temsil eder.

```csharp
public enum HeaderFooterCommandType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Text | `0` | Metin. |
| CurrentPage | `1` | Geçerli sayfa numarası |
| Pagecount | `2` | Sayfa sayısı |
| CurrentDate | `3` | Geçerli tarih |
| CurrentTime | `4` | Geçerli zaman |
| SheetName | `5` | Sayfa adı |
| FileName | `6` | Yol olmadan dosya adı |
| FilePath | `7` | Dosya adı olmadan dosya yolu |
| Picture | `8` | Resim |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHeaderFooterCommandTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Farklı komut tipleriyle başlık ayarla
                worksheet.PageSetup.SetHeader(0, "&[Page] of &[Pages] - &[Date] - &[Time] - &[File]");

                // Başlık komutlarını al
                string headerScript = worksheet.PageSetup.GetHeader(0);
                HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(headerScript);

                // Farklı HeaderFooterCommandType değerlerini göster
                foreach (HeaderFooterCommand cmd in commands)
                {
                    Console.WriteLine($"Command Type: {cmd.Type}");

                    // Belirli komut tiplerini kontrol et
                    if (cmd.Type == HeaderFooterCommandType.CurrentPage)
                    {
                        Console.WriteLine("Found CurrentPage command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.Pagecount)
                    {
                        Console.WriteLine("Found Pagecount command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentDate)
                    {
                        Console.WriteLine("Found CurrentDate command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentTime)
                    {
                        Console.WriteLine("Found CurrentTime command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.FileName)
                    {
                        Console.WriteLine("Found FileName command");
                    }
                }

                // Başlık yapılandırmasını göstermek için çalışma kitabını kaydet
                workbook.Save("HeaderFooterCommandTypeDemo.xlsx");
                Console.WriteLine("HeaderFooterCommandType demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HeaderFooterCommandType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


