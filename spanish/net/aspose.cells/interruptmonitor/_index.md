---
title: "Clase InterruptMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.InterruptMonitor. Representa todo el operador sobre la interrupción"
type: docs
url: /es/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

Representa todos los operadores del interruptor.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | Marca el monitor como solicitando interrupción |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Cuando el procedimiento es interrumpido, si se termina el procedimiento silenciosamente o se lanza una excepción. El valor predeterminado es false, es decir, cuando [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) es true, se lanzará una [`CellsException`](../cellsexception/) con el código Interrupted. (Heredado de [`AbstractInterruptMonitor`](../abstractinterruptmonitor/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | Interrumpe el operador actual. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassInterruptMonitorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Crea y asigna el monitor de interrupción
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Simula la interrupción de la operación
                monitor.Interrupt();
                
                // Intenta guardar (debería ser interrumpido)
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Save completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted.");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### Ver también

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


