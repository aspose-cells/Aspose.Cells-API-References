---
title: "Clase SystemTimeInterruptMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.SystemTimeInterruptMonitor. Implementación simple de AbstractInterruptMonitor mediante la verificación y comparación del tiempo del sistema actual con el límite especificado por el usuario"
type: docs
url: /es/net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

Implementación simple de [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) mediante la verificación y comparación del tiempo del sistema actual con el límite especificado por el usuario.

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | Construye un monitor de interrupción. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | Esta implementación solo verifica si el tiempo consumido (desde el momento en que se inicia este monitor hasta ahora) es mayor que el límite especificado por el usuario. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | Vea [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Esta propiedad es especificada por el usuario al construir esta instancia de monitor. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | Inicia el monitor con el límite de tiempo especificado. El tiempo de inicio para calcular el tiempo consumido es justo cuando se llama a este método, por lo que el procedimiento que necesita ser monitorizado debe iniciarse justo después de esta llamada. |

### Observaciones

Esta implementación es solo una solución simple para escenarios simples. Necesita recuperar y verificar frecuentemente el tiempo del sistema, por lo que puede tener un impacto negativo en el rendimiento en cierta medida.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorDemo
    {
        public static void SystemTimeInterruptMonitorExample()
        {
            // Cree una instancia de SystemTimeInterruptMonitor con terminateWithoutException establecido en false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Cree LoadOptions y establezca InterruptMonitor al monitor creado
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Inicie la monitorización con un límite de tiempo de 1000 milisegundos (1 segundo)
            monitor.StartMonitor(1000);

            try
            {
                // Cargue un libro de trabajo con los LoadOptions especificados
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Si el tiempo de carga del archivo de plantilla supera un segundo, se requerirá una interrupción y se lanzará una excepción aquí
                // De lo contrario, comience a monitorizar el procedimiento de guardado con un nuevo límite de tiempo
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // Guarda el libro de trabajo
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


