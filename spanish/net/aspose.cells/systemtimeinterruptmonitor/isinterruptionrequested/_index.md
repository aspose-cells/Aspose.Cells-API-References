---
title: "SystemTimeInterruptMonitor.IsInterruptionRequested"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SystemTimeInterruptMonitor. Esta implementación solo verifica si el costo de tiempo desde el momento en que se inicia este monitor hasta ahora es mayor que el límite especificado por el usuario"
type: docs
url: /es/net/aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/
---
## SystemTimeInterruptMonitor.IsInterruptionRequested property

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

    public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de SystemTimeInterruptMonitor
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            
            // Iniciar la monitorización con un límite de tiempo de 5 segundos
            monitor.StartMonitor(5000);

            // Mostrar el valor inicial de IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Simular una operación de larga duración
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100000; i++)
            {
                worksheet.Cells[i, 0].Value = i;
                
                // Verificar si se solicitó una interrupción
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation interrupted after time limit!");
                    break;
                }
            }

            // Mostrar el valor final de IsInterruptionRequested
            Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Guardar el resultado
            workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


