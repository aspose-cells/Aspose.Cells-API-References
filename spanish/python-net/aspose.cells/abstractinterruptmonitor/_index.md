---
title: AbstractInterruptMonitor clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---
##  AbstractInterruptMonitor clase
Supervise las solicitudes de interrupción en todas las operaciones que requieren mucho tiempo.



El tipo AbstractInterruptMonitor expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [is_interruption_requested](/cells/es/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) | Indica si se solicita interrupción para la operación actual.<br/>Si es verdadero, se interrumpirá la operación actual.<br/> La implementación debe realizar una verificación rápida y eficiente aquí, de lo contrario, puede convertirse en otro cuello de botella para el procedimiento.|
| [terminate_without_exception](/cells/es/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) | Cuando se interrumpe el procedimiento, ya sea que finalice el procedimiento en silencio o emita una excepción.<br/>El valor predeterminado es falso, es decir, cuando [AbstractInterruptMonitor.is_interruption_requested](/cells/es/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) es verdadero,<br/> Se lanzará un [CellsException](/cells/es/python-net/aspose.cells/cellsexception) con el código [ExceptionType.INTERRUPTED](/cells/es/python-net/aspose.cells/exceptiontype#INTERRUPTED).|



###  Ver también
* módulo [aspose.cells](..)
* clase [CellsException](/cells/es/python-net/aspose.cells/cellsexception)
