---
title: "ThreadInterruptMonitor.FinishMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ThreadInterruptMonitor. Finaliza el monitor para un procedimiento"
type: docs
url: /es/net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

Finaliza el monitor para un procedimiento.

```csharp
public void FinishMonitor()
```

### Observaciones

Llamar a este método después del procedimiento monitorizado puede liberar el hilo del monitor antes, especialmente cuando no hay interrupción para él (el tiempo de ejecución de ese procedimiento es menor que el límite de tiempo especificado).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodFinishMonitorDemo
    {
        public static void Run()
        {
            // Crear una instancia de ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Crear LoadOptions y establecer el InterruptMonitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Iniciar la monitorización con un tiempo de espera de 1 segundo
            monitor.StartMonitor(1000);

            try
            {
                // Simular una operación de larga duración
                for (int i = 0; i < 5; i++)
                {
                    System.Threading.Thread.Sleep(200);
                    Console.WriteLine($"Processing step {i + 1}");
                }

                // Finalizar la monitorización de la operación
                monitor.FinishMonitor();
                Console.WriteLine("Operation completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


