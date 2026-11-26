---
title: "IWarningCallback.Warning"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IWarningCallback. Наш обратный вызов должен реализовать только метод Warning"
type: docs
url: /ru/net/aspose.cells/iwarningcallback/warning/
---
## IWarningCallback.Warning method

Наш обратный вызов должен реализовать только метод "Warning".

```csharp
public void Warning(WarningInfo warningInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| warningInfo | WarningInfo | информация о предупреждении |

### Примеры

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
                
                // Продемонстрировать эффект, сохранив с потенциальным сценарием предупреждения
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

### См. также

* class [WarningInfo](../../warninginfo/)
* interface [IWarningCallback](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


