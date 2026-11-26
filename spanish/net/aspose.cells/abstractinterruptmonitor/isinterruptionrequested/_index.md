---
title: "AbstractInterruptMonitor.IsInterruptionRequested"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractInterruptMonitor. Indica si se solicita una interrupción para la operación actual. Si es true, la operación actual será interrumpida. La implementación debe realizar una verificación rápida y eficiente aquí, de lo contrario podría convertirse en otro cuello de botella para el procedimiento"
type: docs
url: /es/net/aspose.cells/abstractinterruptmonitor/isinterruptionrequested/
---
## AbstractInterruptMonitor.IsInterruptionRequested property

Indica si se solicita una interrupción para la operación actual. Si es true, la operación actual será interrumpida. La implementación debe realizar una verificación rápida y eficiente aquí, de lo contrario podría convertirse en otro cuello de botella para el procedimiento.

```csharp
public abstract bool IsInterruptionRequested { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;
    using System.Threading.Tasks;

    public class AbstractInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear monitor de interrupción y asignarlo al libro de trabajo
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Mostrar valor inicial
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Iniciar tarea de interrupción
            Task.Run(() =>
            {
                Thread.Sleep(1000); // Wait 1 seconds
                Console.WriteLine("\nTriggering interruption...");
                monitor.Interrupt();
            });

            // Simulación de operación de larga duración
            Console.WriteLine("Starting data generation...");
            try
            {
                for (int i = 0; i < 500000000; i++)
                {
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine($"\nInterrupted at row {i}");
                        break;
                    }

                    worksheet.Cells[i, 0].Value = $"Data {i}";
                    
                    // Simular tiempo de procesamiento
                    if (i % 1000 == 0) 
                        Console.Write(".");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("\nError: " + ex.Message);
            }

            // Guardar resultado
            workbook.Save("InterruptionDemoOutput.xlsx");

            Console.WriteLine("\nWorkbook saved with partial data.");
        }
    }
}
```

### Ver también

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


