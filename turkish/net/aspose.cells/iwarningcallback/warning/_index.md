---
title: "IWarningCallback.Warning"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IWarningCallback yöntemi. Geri çağırmamızın yalnızca Warning yöntemini uygulaması gerekir"
type: docs
url: /tr/net/aspose.cells/iwarningcallback/warning/
---
## IWarningCallback.Warning method

Geri çağırmamızın yalnızca "Warning" metodunu uygulaması gerekir.

```csharp
public void Warning(WarningInfo warningInfo)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| warningInfo | WarningInfo | uyarı bilgisi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackMethodWarningWithWarningInfoDemo : IWarningCallback
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var demo = new IWarningCallbackMethodWarningWithWarningInfoDemo();
            workbook.Settings.WarningCallback = demo;

            try
            {
                Console.WriteLine("Warning callback is set up. Any warnings during operations will be displayed.");
                
                // Potansiyel bir uyarı senaryosu ile kaydederek etkiyi göster
                worksheet.Cells["A1"].Formula = "=1/0"; // This may trigger a warning
                workbook.Save("WarningDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning Type: {warningInfo.Type}");
            Console.WriteLine($"Description: {warningInfo.Description}");
            Console.WriteLine($"Corrected Object: {warningInfo.CorrectedObject ?? "null"}");
        }
    }
}
```

### Ayrıca Bakınız

* class [WarningInfo](../../warninginfo/)
* interface [IWarningCallback](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


