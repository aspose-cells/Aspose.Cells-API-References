---
title: AbstractInterruptMonitor klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 50
url: /sv/python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---
##  AbstractInterruptMonitor klass
Övervaka för avbrutna förfrågningar i alla tidskrävande operationer.



Typen AbstractInterruptMonitor avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [is_interruption_requested](/cells/sv/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) | Indikerar om avbrott begärs för aktuell drift.<br/>Om sant kommer den aktuella driften att avbrytas.<br/>Implementeringen bör utföra snabb och effektiv kontroll här, annars kan det bli ytterligare en flaskhals för proceduren.|
| [terminate_without_exception](/cells/sv/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) | När proceduren avbryts, om man ska avsluta proceduren tyst eller göra ett undantag.<br/>Standard är falskt, det vill säga när [AbstractInterruptMonitor.is_interruption_requested](/cells/sv/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) är sant,<br/> ett [CellsException](/cells/sv/python-net/aspose.cells/cellsexception) med kod [ExceptionType.INTERRUPTED](/cells/sv/python-net/aspose.cells/exceptiontype#INTERRUPTED) kommer att kastas.|



###  Se även
* modul [aspose.cells](..)
* klass [CellsException](/cells/sv/python-net/aspose.cells/cellsexception)
