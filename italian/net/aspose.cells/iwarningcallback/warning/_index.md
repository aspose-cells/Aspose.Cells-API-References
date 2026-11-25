---
title: "IWarningCallback.Warning"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IWarningCallback. Il nostro callback deve implementare solo il metodo Warning"
type: docs
url: /it/net/aspose.cells/iwarningcallback/warning/
---
## IWarningCallback.Warning method

Il nostro callback deve solo implementare il metodo \"Warning\".

```csharp
public void Warning(WarningInfo warningInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| warningInfo | WarningInfo | informazioni di avviso |

### Esempi

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
                
                // Dimostra l'effetto salvando con uno scenario di avviso potenziale
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

### Vedi anche

* class [WarningInfo](../../warninginfo/)
* interface [IWarningCallback](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


