---
title: "SystemTimeInterruptMonitor.SystemTimeInterruptMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de SystemTimeInterruptMonitor. Construye un monitor de interrupción"
type: docs
url: /es/net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

Construye un monitor de interrupción.

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Crear una instancia con terminateWithoutException establecido en false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Configurar opciones de carga con el monitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Iniciar monitoreo con un límite de tiempo de 1 segundo
            monitor.StartMonitor(1000);

            try
            {
                // Intentar cargar un libro de trabajo
                Workbook wb = new Workbook("sample.xlsx", lopts);

                // Restablecer el monitor para la operación de guardado con un límite de 1.5 segundos
                monitor.StartMonitor(1500);
                wb.Save("output.xlsx");
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

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


