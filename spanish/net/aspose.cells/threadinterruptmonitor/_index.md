---
title: "Clase ThreadInterruptMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ThreadInterruptMonitor. Implementación simple de AbstractInterruptMonitor iniciando otro hilo para requerir la interrupción después de dormir el límite especificado por el usuario"
type: docs
url: /es/net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

Implementación simple de [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) iniciando otro hilo para requerir la interrupción después de dormir el límite especificado por el usuario.

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | Construye un monitor de interrupción. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | Esta implementación solo verifica si el tiempo consumido (desde el momento en que se inicia este monitor hasta ahora) es mayor que el límite especificado por el usuario. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | Vea [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Esta propiedad es especificada por el usuario al construir esta instancia de monitor. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | Finaliza el monitor para un procedimiento. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | Inicia el monitor con el límite de tiempo especificado. El tiempo de inicio para calcular el tiempo consumido es justo cuando se llama a este método, por lo que el procedimiento que necesita ser monitorizado debe iniciarse justo después de esta llamada. |

### Observaciones

Una instancia del monitor puede usarse repetidamente, siempre que monitorees cada proceso en secuencia. No debe usarse para monitorear varios procedimientos simultáneamente en múltiples hilos.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorDemo
    {
        public static void ThreadInterruptMonitorExample()
        {
            // Crea una instancia de ThreadInterruptMonitor con terminateWithoutException establecido en false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Cree LoadOptions y establezca InterruptMonitor al monitor creado
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Inicia el monitor con un límite de tiempo de 1000 milisegundos (1 segundo)
            monitor.StartMonitor(1000);

            try
            {
                // Cargue un libro de trabajo con los LoadOptions especificados
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Finaliza el monitor para el procedimiento de carga
                monitor.FinishMonitor();

                // Inicia el monitor nuevamente con un nuevo límite de tiempo de 1500 milisegundos (1.5 segundos)
                monitor.StartMonitor(1500);

                // Guarda el libro de trabajo
                wb.Save("result.xlsx");

                // Finaliza el monitor para el procedimiento de guardado
                monitor.FinishMonitor();
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

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


