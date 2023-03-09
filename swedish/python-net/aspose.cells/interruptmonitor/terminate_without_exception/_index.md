---
title: terminate_without_exception fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 50
url: /sv/python-net/aspose.cells/interruptmonitor/terminate_without_exception/
is_root: false
---
##  terminate_without_exception fastighet

När proceduren avbryts, om man ska avsluta proceduren tyst eller göra ett undantag.
Standard är falskt, det vill säga när [AbstractInterruptMonitor.is_interruption_requested](/cells/sv/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) är sant,
ett [CellsException](/cells/sv/python-net/aspose.cells/cellsexception) med kod [ExceptionType.INTERRUPTED](/cells/sv/python-net/aspose.cells/exceptiontype#INTERRUPTED) kommer att kastas.
###  Definition:
```python
@property
def terminate_without_exception(self):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [CellsException](/cells/sv/python-net/aspose.cells/cellsexception)
* klass [InterruptMonitor](/cells/sv/python-net/aspose.cells/interruptmonitor)
