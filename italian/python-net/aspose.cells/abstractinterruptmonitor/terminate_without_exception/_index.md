---
title: terminate_without_exception proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception/
is_root: false
---
##  terminate_without_exception proprietà

Quando la procedura viene interrotta, se terminare la procedura in silenzio o lanciare un'eccezione.
L'impostazione predefinita è false, ovvero quando [AbstractInterruptMonitor.is_interruption_requested](/cells/it/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) è vero,
verrà lanciato uno [CellsException](/cells/it/python-net/aspose.cells/cellsexception) con codice [ExceptionType.INTERRUPTED](/cells/it/python-net/aspose.cells/exceptiontype#INTERRUPTED).
###  Definizione:
```python
@property
def terminate_without_exception(self):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [AbstractInterruptMonitor](/cells/it/python-net/aspose.cells/abstractinterruptmonitor)
* classe [CellsException](/cells/it/python-net/aspose.cells/cellsexception)
