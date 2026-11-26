---
title: "ThreadInterruptMonitor.TerminateWithoutException"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadInterruptMonitor. Ver TerminateWithoutException. Esta propiedad es especificada por el usuario al construir esta instancia del monitor"
type: docs
url: /es/net/aspose.cells/threadinterruptmonitor/terminatewithoutexception/
---
## ThreadInterruptMonitor.TerminateWithoutException property

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

    public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de ThreadInterruptMonitor con el valor inicial de TerminateWithoutException
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            
            // Mostrar el valor actual de la propiedad
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Iniciar monitoreo con un límite de 5 segundos
            monitor.StartMonitor(5000);

            // Demostrar el procesamiento que podría ser interrumpido
            try
            {
                for (int i = 0; i < 100000; i++)
                {
                    // Simular un procesamiento largo
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Processing was interrupted");
                        break;
                    }
                    worksheet.Cells[i, 0].Value = "Value " + i;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception occurred: " + ex.Message);
            }
            finally
            {
                monitor.FinishMonitor();
            }

            // Crear otro monitor con TerminateWithoutException establecido en true
            ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
            Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);

            // Guardar el resultado
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


