---
title: terminate_without_exception propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells/interruptmonitor/terminate_without_exception/
is_root: false
---
##  terminate_without_exception propiedad

Cuando se interrumpe el procedimiento, ya sea que finalice el procedimiento en silencio o emita una excepción.
El valor predeterminado es falso, es decir, cuando [AbstractInterruptMonitor.is_interruption_requested](/cells/es/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) es verdadero,
Se lanzará un [CellsException](/cells/es/python-net/aspose.cells/cellsexception) con el código [ExceptionType.INTERRUPTED](/cells/es/python-net/aspose.cells/exceptiontype#INTERRUPTED).
###  Definición:
```python
@property
def terminate_without_exception(self):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [CellsException](/cells/es/python-net/aspose.cells/cellsexception)
* clase [InterruptMonitor](/cells/es/python-net/aspose.cells/interruptmonitor)
