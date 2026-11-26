---
title: "IWarningCallback.Warning"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IWarningCallback. Nuestro callback solo necesita implementar el método Warning"
type: docs
url: /es/net/aspose.cells/iwarningcallback/warning/
---
## IWarningCallback.Warning method

Nuestro callback solo necesita implementar el método "Warning".

```csharp
public void Warning(WarningInfo warningInfo)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| warningInfo | WarningInfo | información de advertencia |

### Ejemplos

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
                
                // Demostrar el efecto guardando con un posible escenario de advertencia
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

### Ver también

* class [WarningInfo](../../warninginfo/)
* interface [IWarningCallback](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


