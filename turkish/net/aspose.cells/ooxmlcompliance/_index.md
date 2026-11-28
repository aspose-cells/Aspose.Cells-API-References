---
title: "Enum OoxmlCompliance"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.OoxmlCompliance enum. Xlsx formatında kaydederken kullanılacak OOXML spesifikasyonunu belirtmeye olanak tanır"
type: docs
url: /tr/net/aspose.cells/ooxmlcompliance/
---
## OoxmlCompliance enumeration

Xlsx formatında kaydederken hangi OOXML spesifikasyonunun kullanılacağını belirtmeye izin verir.

```csharp
public enum OoxmlCompliance
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Ecma376_2006 | `0` | ECMA-376 1. Baskı, 2006. |
| Iso29500_2008_Strict | `1` | ISO/IEC 29500:2008 Katı uyumluluk seviyesi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlComplianceDemo
    {
        public static void OoxmlComplianceExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // OOXML uyumluluk seviyesini ISO/IEC 29500:2008 Katı olarak ayarla
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;

            // Çalışma sayfasına bazı veriler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, World!");

            // Belirtilen OOXML uyumluluk seviyesiyle çalışma kitabını kaydet
            workbook.Save("OoxmlComplianceExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


