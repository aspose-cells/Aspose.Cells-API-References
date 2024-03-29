---
title: InterruptMonitor
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa a todos los operadores sobre la interrupción.
type: docs
weight: 3910
url: /es/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

Representa a todos los operadores sobre la interrupción.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [InterruptMonitor](interruptmonitor)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested) { get; } | Marcar el monitor como solicitando interrupción |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception) { get; } | Cuando se interrumpe el procedimiento, ya sea que finalice el procedimiento silenciosamente o arroje una excepción. El valor predeterminado es falso, es decir, cuando[`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested) es cierto, a[`CellsException`](../cellsexception) con codigoInterrupted será lanzado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt)() | Interrumpir al operador actual. |

### Ver también

* class [AbstractInterruptMonitor](../abstractinterruptmonitor)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
