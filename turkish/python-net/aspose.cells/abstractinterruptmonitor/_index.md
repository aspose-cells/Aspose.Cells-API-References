---
title: AbstractInterruptMonitor sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 50
url: /tr/python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---
##  AbstractInterruptMonitor sınıfı
Zaman alan tüm işlemlerde kesintiye uğrayan istekleri izleyin.



AbstractInterruptMonitor türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [is_interruption_requested](/cells/tr/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) | Geçerli işlem için kesinti istenip istenmediğini gösterir.<br/>Doğru ise, mevcut işlem kesintiye uğrayacaktır.<br/>Uygulama burada hızlı ve verimli kontrol yapmalıdır, aksi takdirde prosedür için başka bir darboğaza dönüşebilir.|
| [terminate_without_exception](/cells/tr/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) | Prosedür kesintiye uğradığında, prosedürü sessizce sonlandırmak veya bir İstisna atmak.<br/>Varsayılan yanlıştır, yani [AbstractInterruptMonitor.is_interruption_requested](/cells/tr/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) doğru olduğunda,<br/> [ExceptionType.INTERRUPTED](/cells/tr/python-net/aspose.cells/exceptiontype#INTERRUPTED) kodlu bir [CellsException](/cells/tr/python-net/aspose.cells/cellsexception) atılacak.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [CellsException](/cells/tr/python-net/aspose.cells/cellsexception)
