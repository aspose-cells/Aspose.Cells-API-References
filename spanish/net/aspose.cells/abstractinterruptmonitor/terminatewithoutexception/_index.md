---
title: "AbstractInterruptMonitor.TerminateWithoutException"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractInterruptMonitor. Cuando el procedimiento se interrumpe, si se debe terminar el procedimiento silenciosamente o lanzar una Exception. El valor predeterminado es false, es decir, cuando IsInterruptionRequested es true se lanzará una CellsException con el código Interrupted."
type: docs
url: /es/net/aspose.cells/abstractinterruptmonitor/terminatewithoutexception/
---
## AbstractInterruptMonitor.TerminateWithoutException property

Cuando el procedimiento se interrumpe, si se debe terminar el procedimiento silenciosamente o lanzar una Exception. El valor predeterminado es false, es decir, cuando [`IsInterruptionRequested`](../isinterruptionrequested/) es true, se lanzará una [`CellsException`](../../cellsexception/) con el código Interrupted.

```csharp
public virtual bool TerminateWithoutException { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar la hoja de cálculo para crear carga de procesamiento
            for (int row = 0; row < 5000; row++)
            {
                for (int col = 0; col < 50; col++)
                {
                    worksheet.Cells[row, col].Value = "SampleData";
                }
            }

            // Demostrar SystemTimeInterruptMonitor con terminación por excepción
            var interruptMonitor1 = new SystemTimeInterruptMonitor(terminateWithoutException: false);
            Console.WriteLine($"Initial TerminateWithoutException: {interruptMonitor1.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor1;
            interruptMonitor1.StartMonitor(1); // Set 1ms timeout

            try
            {
                workbook.Save("TerminateWithException.xlsx");
                Console.WriteLine("Saved successfully (unexpected with false setting)");
            }
            catch (CellsException ex)
            {
                Console.WriteLine($"Operation terminated with exception: {ex.Message}");
            }

            // Demostrar SystemTimeInterruptMonitor con terminación silenciosa
            var interruptMonitor2 = new SystemTimeInterruptMonitor(terminateWithoutException: true);
            Console.WriteLine($"\nNew TerminateWithoutException: {interruptMonitor2.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor2;
            interruptMonitor2.StartMonitor(1);

            try
            {
                workbook.Save("TerminateSilently.xlsx");
                Console.WriteLine("Saved without exception (expected with true setting)");
            }
            catch (CellsException)
            {
                Console.WriteLine("Exception caught (unexpected with true setting)");
            }

        }
    }

}
```

### Ver también

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


