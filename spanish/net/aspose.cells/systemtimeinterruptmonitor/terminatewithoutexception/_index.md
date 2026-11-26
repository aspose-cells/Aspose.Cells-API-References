---
title: "SystemTimeInterruptMonitor.TerminateWithoutException"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SystemTimeInterruptMonitor. Ver TerminateWithoutException. Esta propiedad es especificada por el usuario al crear esta instancia del monitor."
type: docs
url: /es/net/aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/
---
## SystemTimeInterruptMonitor.TerminateWithoutException property

Ver [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/). Esta propiedad es especificada por el usuario al crear esta instancia del monitor.

```csharp
public override bool TerminateWithoutException { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de SystemTimeInterruptMonitor con el valor inicial de TerminateWithoutException
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Mostrar el valor actual de la propiedad TerminateWithoutException
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Iniciar la monitorización con un límite de tiempo de 1000 ms
            monitor.StartMonitor(1000);

            // Demostrar el efecto de TerminateWithoutException intentando una operación larga
            try
            {
                // Simular una operación larga que podría exceder el límite de tiempo
                for (int i = 0; i < 100000; i++)
                {
                    worksheet.Cells[i, 0].Value = i;
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Operation interrupted by monitor");
                        break;
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception caught: " + ex.Message);
            }

            // Crear otro monitor con TerminateWithoutException establecido en true
            SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
            Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);

            // Guarda el libro de trabajo
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


