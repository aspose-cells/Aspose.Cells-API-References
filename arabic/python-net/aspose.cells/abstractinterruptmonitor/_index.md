---
title: AbstractInterruptMonitor الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 50
url: /ar/python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---
##  AbstractInterruptMonitor الدرجة
مراقبة طلبات الانقطاع في جميع العمليات التي تستغرق وقتًا طويلاً.



يكشف نوع AbstractInterruptMonitor الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [is_interruption_requested](/cells/ar/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) | يشير إلى ما إذا كان الانقطاع مطلوبًا للعملية الحالية.<br/>إذا كان هذا صحيحًا ، فستتوقف العملية الحالية.<br/>يجب أن يتم تنفيذ الفحص بسرعة وكفاءة هنا ، وإلا فقد يصبح عنق الزجاجة آخر للإجراء.|
| [terminate_without_exception](/cells/ar/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) | عند مقاطعة الإجراء ، سواء إنهاء الإجراء بهدوء أو طرح استثناء.<br/>الافتراضي خطأ ، أي عندما يكون [AbstractInterruptMonitor.is_interruption_requested](/cells/ar/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) صحيحًا ،<br/> سيتم طرح [CellsException](/cells/ar/python-net/aspose.cells/cellsexception) برمز [ExceptionType.INTERRUPTED](/cells/ar/python-net/aspose.cells/exceptiontype#INTERRUPTED).|



###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [CellsException](/cells/ar/python-net/aspose.cells/cellsexception)
