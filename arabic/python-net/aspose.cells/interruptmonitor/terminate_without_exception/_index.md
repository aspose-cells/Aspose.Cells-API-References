---
title: terminate_without_exception الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 50
url: /ar/python-net/aspose.cells/interruptmonitor/terminate_without_exception/
is_root: false
---
##  terminate_without_exception الملكية

عند مقاطعة الإجراء ، سواء إنهاء الإجراء بهدوء أو طرح استثناء.
الافتراضي خطأ ، أي عندما يكون [AbstractInterruptMonitor.is_interruption_requested](/cells/ar/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) صحيحًا ،
سيتم طرح [CellsException](/cells/ar/python-net/aspose.cells/cellsexception) برمز [ExceptionType.INTERRUPTED](/cells/ar/python-net/aspose.cells/exceptiontype#INTERRUPTED).
###  تعريف:
```python
@property
def terminate_without_exception(self):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [CellsException](/cells/ar/python-net/aspose.cells/cellsexception)
* فئة [InterruptMonitor](/cells/ar/python-net/aspose.cells/interruptmonitor)
