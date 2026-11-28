---
title: "Arayüz IWarningCallback"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.IWarningCallback arayüzü. Uyarı geri çağırma arayüzü."
type: docs
url: /tr/net/aspose.cells/iwarningcallback/
---
## IWarningCallback interface

Uyarı geri çağırma arayüzü.

```csharp
public interface IWarningCallback
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Warning](../../aspose.cells/iwarningcallback/warning/)(WarningInfo) | Geri çağırmamızın yalnızca "Warning" metodunu uygulaması gerekir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackDemo : IWarningCallback
    {
        // IWarningCallback arayüzünden Warning metodunu uygulama
        public void Warning(WarningInfo warningInfo)
        {
            // Uyarı mesajını göster.
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
        }

        public static void IWarningCallbackExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Uyarı geri çağırmasını ayarla.
            workbook.Settings.WarningCallback = new IWarningCallbackDemo();

            // Olası uyarılar içeren bir çalışma kitabı yükle.
            try
            {
                workbook = new Workbook("example.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("IWarningCallbackExample.xlsx");
        }
    }

}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


