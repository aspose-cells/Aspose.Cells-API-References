---
title: "Enum SensitivityLabelMarkType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Metas.SensitivityLabelMarkType enum. Bir dosyaya uygulanması gereken içerik işaretleme türlerini temsil eder"
type: docs
url: /tr/net/aspose.cells.metas/sensitivitylabelmarktype/
---
## SensitivityLabelMarkType enumeration

Bir dosyaya uygulanması gereken içerik işaretleme türlerini temsil eder.

```csharp
[Flags]
public enum SensitivityLabelMarkType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Yok |
| Header | `1` | Üstbilgi |
| Footer | `2` | Altbilgi |
| Watermark | `4` | Filigran |
| Encryption | `8` | Şifreleme |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelMarkTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SensitivityLabelMarkType enum değerlerini gösterin
            SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;

            // Türüne göre farklı hassasiyet etiketi işaretlerini uygulayın
            switch (markType)
            {
                case SensitivityLabelMarkType.None:
                    Console.WriteLine("No sensitivity label applied");
                    break;
                case SensitivityLabelMarkType.Header:
                    worksheet.PageSetup.SetHeader(0, "CONFIDENTIAL");
                    break;
                case SensitivityLabelMarkType.Footer:
                    worksheet.PageSetup.SetFooter(0, "INTERNAL USE ONLY");
                    break;
                case SensitivityLabelMarkType.Watermark:
                    worksheet.PageSetup.SetHeader(0, "&KFF0000&DRAFT");
                    break;
                case SensitivityLabelMarkType.Encryption:
                    workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
                    break;
            }

            // Uygulanan hassasiyet etiketiyle çalışma kitabını kaydedin
            workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


