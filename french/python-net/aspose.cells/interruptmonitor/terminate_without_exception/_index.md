---
title: terminate_without_exception propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 50
url: /fr/python-net/aspose.cells/interruptmonitor/terminate_without_exception/
is_root: false
---
##  terminate_without_exception propriété

Lorsque la procédure est interrompue, qu'elle soit terminée silencieusement ou qu'elle lève une exception.
La valeur par défaut est false, c'est-à-dire que lorsque [AbstractInterruptMonitor.is_interruption_requested](/cells/fr/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) est vrai,
un [CellsException](/cells/fr/python-net/aspose.cells/cellsexception) avec le code [ExceptionType.INTERRUPTED](/cells/fr/python-net/aspose.cells/exceptiontype#INTERRUPTED) sera lancé.
###  Définition:
```python
@property
def terminate_without_exception(self):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [CellsException](/cells/fr/python-net/aspose.cells/cellsexception)
* classe [InterruptMonitor](/cells/fr/python-net/aspose.cells/interruptmonitor)
