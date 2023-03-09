---
title: InterruptMonitor clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 950
url: /es/python-net/aspose.cells/interruptmonitor/
is_root: false
---
##  InterruptMonitor clase
Representa a todos los operadores sobre la interrupción.



**Herencia:** [InterruptMonitor](/cells/python-net/aspose.cells/interruptmonitor) → 
[AbstractInterruptMonitor](/cells/es/python-net/aspose.cells/abstractinterruptmonitor)



El tipo InterruptMonitor expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [InterruptMonitor()](/cells/es/python-net/aspose.cells/interruptmonitor/__init__/#) | Construye una nueva instancia de InterruptMonitor|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [is_interruption_requested](/cells/es/python-net/aspose.cells/interruptmonitor/is_interruption_requested) | Marcar el monitor como solicitando interrupción|
| [terminate_without_exception](/cells/es/python-net/aspose.cells/interruptmonitor/terminate_without_exception) | Cuando se interrumpe el procedimiento, ya sea que finalice el procedimiento en silencio o emita una excepción.<br/>El valor predeterminado es falso, es decir, cuando [AbstractInterruptMonitor.is_interruption_requested](/cells/es/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) es verdadero,<br/> Se lanzará un [CellsException](/cells/es/python-net/aspose.cells/cellsexception) con el código [ExceptionType.INTERRUPTED](/cells/es/python-net/aspose.cells/exceptiontype#INTERRUPTED).|


###  Métodos
| Método| Descripción|
| :- | :- |
| [interrupt()](/cells/es/python-net/aspose.cells/interruptmonitor/interrupt/#) | Interrumpir al operador actual.|



###  Ver también
* módulo [aspose.cells](..)
* clase [AbstractInterruptMonitor](/cells/es/python-net/aspose.cells/abstractinterruptmonitor)
* clase [CellsException](/cells/es/python-net/aspose.cells/cellsexception)
* clase [InterruptMonitor](/cells/es/python-net/aspose.cells/interruptmonitor)
