---
title: "ThreadInterruptMonitor.IsInterruptionRequested"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadInterruptMonitor. Esta implementación solo verifica si el tiempo transcurrido desde que se inició este monitor hasta ahora es mayor que el límite especificado por el usuario"
type: docs
url: /es/net/aspose.cells/threadinterruptmonitor/isinterruptionrequested/
---
## ThreadInterruptMonitor.IsInterruptionRequested property

Esta implementación solo verifica si el tiempo consumido (desde el momento en que se inicia este monitor hasta ahora) es mayor que el límite especificado por el usuario.

```csharp
public override bool IsInterruptionRequested { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;

    public class ThreadInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);

            // Iniciar monitoreo con un límite de 2 segundos
            monitor.StartMonitor(2000);

            // Simular una operación de larga duración
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100; i++)
            {
                // Verificar si se solicitó una interrupción
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation was interrupted!");
                    break;
                }

                // Simular trabajo
                Thread.Sleep(100);
                worksheet.Cells[i, 0].Value = $"Processed row {i}";
                Console.WriteLine($"Processed row {i}");
            }

            // Finalizar monitoreo
            monitor.FinishMonitor();

            // Guardar el resultado
            workbook.Save("ThreadInterruptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


