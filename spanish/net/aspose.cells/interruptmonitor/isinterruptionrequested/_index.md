---
title: "InterruptMonitor.IsInterruptionRequested"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad InterruptMonitor. Marca el monitor como solicitando interrupción"
type: docs
url: /es/net/aspose.cells/interruptmonitor/isinterruptionrequested/
---
## InterruptMonitor.IsInterruptionRequested property

Marca el monitor como solicitando interrupción

```csharp
public override bool IsInterruptionRequested { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a su primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un monitor de interrupción y asignarlo al libro de trabajo
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Mostrar el estado inicial de IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested value: " + monitor.IsInterruptionRequested);

            // Simular una operación de procesamiento de datos de larga duración
            Console.WriteLine("Starting data processing...");
            for (int rowIdx = 0; rowIdx < 10000; rowIdx++)
            {
                // Solicitar interrupción después de procesar 500 filas
                if (rowIdx == 500)
                {
                    monitor.Interrupt();
                    Console.WriteLine("Interrupt requested. IsInterruptionRequested: " + monitor.IsInterruptionRequested);
                }

                // Comprobar si hay solicitud de interrupción
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine($"Processing interrupted at row {rowIdx}");
                    break;
                }

                // Simular procesamiento de datos
                worksheet.Cells[rowIdx, 0].Value = $"Row {rowIdx} data";
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("InterruptionDemoOutput.xlsx");
            Console.WriteLine("File saved with partial data due to interruption.");
        }
    }
}
```

### Ver también

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


