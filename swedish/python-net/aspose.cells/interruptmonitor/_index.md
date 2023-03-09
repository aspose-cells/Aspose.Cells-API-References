---
title: InterruptMonitor klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 950
url: /sv/python-net/aspose.cells/interruptmonitor/
is_root: false
---
##  InterruptMonitor klass
Representerar alla operatörer om avbrottet.



**Arv:** [InterruptMonitor](/cells/python-net/aspose.cells/interruptmonitor) → 
[AbstractInterruptMonitor](/cells/sv/python-net/aspose.cells/abstractinterruptmonitor)



Typen InterruptMonitor avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [InterruptMonitor()](/cells/sv/python-net/aspose.cells/interruptmonitor/__init__/#) | Konstruerar en ny instans av InterruptMonitor|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [is_interruption_requested](/cells/sv/python-net/aspose.cells/interruptmonitor/is_interruption_requested) | Markera monitorn som begär avbrott|
| [terminate_without_exception](/cells/sv/python-net/aspose.cells/interruptmonitor/terminate_without_exception) | När proceduren avbryts, oavsett om du avbryter proceduren tyst eller gör ett undantag.<br/>Standard är falskt, det vill säga när [AbstractInterruptMonitor.is_interruption_requested](/cells/sv/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) är sant,<br/> ett [CellsException](/cells/sv/python-net/aspose.cells/cellsexception) med kod [ExceptionType.INTERRUPTED](/cells/sv/python-net/aspose.cells/exceptiontype#INTERRUPTED) kommer att kastas.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [interrupt()](/cells/sv/python-net/aspose.cells/interruptmonitor/interrupt/#) | Avbryt den aktuella operatören.|



###  Se även
* modul [aspose.cells](..)
* klass [AbstractInterruptMonitor](/cells/sv/python-net/aspose.cells/abstractinterruptmonitor)
* klass [CellsException](/cells/sv/python-net/aspose.cells/cellsexception)
* klass [InterruptMonitor](/cells/sv/python-net/aspose.cells/interruptmonitor)
